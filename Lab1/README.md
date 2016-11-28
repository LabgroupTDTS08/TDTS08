# Labroration 1
  1. The array A[] is spatial locality because it has many different elemts close to each other. The loop variables i and j on other hand is just updating from the same position in the memory so it is temporal locality. The same goes for the sum variable.
  2. Test1 with cache1 gives 19 hits between two misses and Test1 witch cache 2 gives 9 hits between misses. Test2 with cache1 gives first two cache misses directly after each other however the second miss will overwrite the first cachemiss data that was stored in the cache because they are stored on the same line. This makes it so we get a cache miss all the time and no hits in between the misses. Test2 with cache 2 gives 19 hits between misses. By these predictions Test1 should be best with case1 while Test2 should be best with case2.
  3. Test1 with cache1 gives 800585 misses, Test1 with cache2 gives 1558207 misses, Test2 with cache1 gives 10596833 misses, Test2 with cache2 gives 1581391. Test1 got the least misses with case1 and Test2 got the least misses with case2 as we predicted. 
  4. For low number of sets the associativity is important for the miss-ratio, but when the sets go up you se that the associativity does not matter so much anymore. The associativity also depends more on data caching , when the associativity gets bigger for instruction caching it does not affect.
  5. By looking at the graphs we see that if only intructions is stored in the cache we get the least amount of cachemisses(missrate about 0,03 %). However we only took in consideration instruction in that case, all the data dependent code will all be ignorde by the cache and be the same as a cache miss. Since half the code is data dependent the missrate becomes at best about 50 % in that case. The unified cache takes both data and instruction in consideration and does gives us a missrate of about 1 % acording to our graph. This makes a unified cache the best one.   
  6. The minimize cost for the intruction cache is for cachesize 128 and associativity 2.
  



## Preperations questions
  1. 2^8 = 256 bytes, blocksize is four bytes which gives two bits are bytenumber. Linenumber are two bits because there is 8 cache lines. The tag is the rest of the 8 bits, 3 bits.
  2. 000110011 = line 6, 00110100 = line 5, 11010000= line 4, 10101010 = line 2, frome above information.
  3. 10100000, 10100010, 10100011 is the other adresses storde in the cache with a miss on 10100001.
  4. Total bytes of the cache is blocke size times number of lines = 32 bytes.
  5. The tag is stored to check if the adress that is going to be used is already in the cache.
  6. From the example code you can see that the string is not called so often like "i", so "i" is in this case probaly a temporal locality and the string "Hello worls" is a spatial locality.
