# Labroration 1
  1. The array A[] is spatial locality because it has many different elemts close to each other. The loop variable i on other hand is just updating from the same position in the memory so it is temporal locality.
  2. Test1 with cache1 gives 19 hits between two misses, Test1 witch cache 2 gives 9 hits between misses, Test2 with cache1 gives 39 hits between misses but have alot of misses in a row at some points, Test2 with cache 2 gives 19 hits between misses.
  3. Test1 with cache1 gives 800585 misses, Test1 witch cache2 gives 1558207 misses, Test2 with cache1 gives 10596833 misses, Test2 with cache2 gives 1581391.
  4. For low number of sets the associativity is important for the miss-ratio, but when the sets go up you se that the associativity does not matter so much anymore. The associativity also depends more on data caching , when the associativity gets bigger for instruction caching it does not affect.
  5. By looking at the graphs we see that if only intructions is stored in the cache we get the least amount of cachemisses, why both do not have the same result depends on that the cache fills up so much faster, otherhand the program problaly gonna be faster if we cache unified..
  6. The minimize cost for the intruction cache is for cachesize 128 and associativity 2.
  



## Preperations questions
  1. 2^8 = 256 bytes, blocksize is four bytes which gives two bits are bytenumber. Linenumber are two bits because there is 8 cache lines. The tag is the rest of the 8 bits, 3 bits.
  2. 000110011 = line 6, 00110100 = line 5, 11010000= line 4, 10101010 = line 2, frome above information.
  3. 10100000, 10100010, 10100011 is the other adresses storde in the cache with a miss on 10100001.
  4. Total bytes of the cache is blocke size times number of lines = 32 bytes.
  5. The tag is stored to check if the adress that is going to be used is already in the cache.
  6. From the example code you can see that the string is not called so often like "i", so "i" is in this case probaly a temporal locality and the string "Hello worls" is a spatial locality.
