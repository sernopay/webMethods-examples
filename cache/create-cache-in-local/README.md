# Create Cache in Local

## Create Cache Manager
1. open wm administrator page
2. click settings -> caching \
![](images/1.png)
3. click add cache manager \
![](images/2.png)
4. let's name it `cache.local.test` -> click `save changes`
5. the created cache managers will be shown in `public cache managers` table. click `start`
![](images/3.png)
6. open the `cache.local.test` 
7. click add cache \
![](images/4.png)
8. let's name the cache name as `cache-test`, `Maximum Elements in Memory` = 100, set `time to live` to `120`, then click `save changes`
![](images/5.png)

## Set the value to the cache
1. create a map to create a `value` lets define it `test-cache` and `key` with value `key-cache` \
![](images/6.png)
![](images/7.png)
2. put the cache using `pub.cache:put` with this configuration
- `cacheManagerName` : `cache.local.test` (cache manager that we created previously)
- `cacheName` : `cache-test` (cache name that we created previously)
- `value` : `value`
- `key` : `key`
![](images/8.png)

## Get the value from the cache
1. create map step to create a `key` with value `key-cache`
2. get the cache using `pub.cache:get` with this configuration
- `cacheManagerName` : `cache.local.test` (cache manager that we created previously)
- `cacheName` : `cache-test` (cache name that we created previously)
- `value` : `value`
- `key` : `key`
![](images/9.png)

# Test the service
1. run the put cache service
![](images/10.png)
2. run the get cache service
![](images/11.png)

as you can see in the cache, the `value` is get from cache