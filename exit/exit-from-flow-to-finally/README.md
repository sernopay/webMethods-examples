- exit $flow will make flow go out from flow, but if you have a finally then it will go to the finally first
- in here if `input` is empty then we will exit from flow, and continue to finally. 
- else it will set `result` to `ok`
![alt text](images/1.png)
- in finally it will set `resultFinally` = ok
![alt text](images/2.png)

Test
- `input` = `null`
![alt text](images/3.png)
![alt text](images/4.png)

as we can see it only set `resultFinally` because the input is null

- `input` != `null`
![alt text](images/5.png)
![alt text](images/6.png)