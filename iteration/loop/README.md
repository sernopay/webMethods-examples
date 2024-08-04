# Loop Example

1. Create a string list as an input, and name it `names` \
![](images/5.jpg)
2. Add loop, and set `Input Array` property to `names` \
![](images/1.jpg)

3. Add `pub.flow.debuglog` service, and set `Message` property to `%$iteration% %names%`. Don't forget to check `Perform pipeline variable substitution` checkbox. \
![](images/2.jpg)

4. Run the service, and check the log in the server log. \
![](images/3.jpg) \
![](images/4.jpg)