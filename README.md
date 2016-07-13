Basic Web Search Engine  

Project Structure:  
1. WikiSearch.java contains main() method where you can enter the search query on System.in.  
2. Currently, WikiSearch does not make a call to the crawler since the crawler has already indexed the URLs the Redis database.  
3. JedisIndex is used by WikiSearch to get the counts of the indexed terms to find relevance.  
4. Although JedisIndex mentions that the index contains only two Wikipedia pages, that does not hold true since I tried to index all of wikipedia.  
5. JedisIndex uses TermCounter to push a map of terms and their counts onto the database.  
6. WikiFetcher is used while crawling Wikipedia to get the DOM elements og the webpage.  

Inside the java folder,  
Compile using --> ant build.  
To run the program --> ant WikiSearch.  

