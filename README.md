# Caching
This report is created to investigate different caching approaches. Various caching methods and their importance are discussed to pick the better caching technique to help the team deploy them efficiently. 

## Introduction 

Caching is a process of storing copies of files locally in a cache or temporary files at a location where the fetching of these data generally becomes faster than fetching from the original source.


Cached data typically includes multimedia such as images, files, and scripts, which are automatically stored on a device the first time a user opens an application or visits a website. This is used to quickly load the application or website’s information every time the user subsequently opens or visits it.

### Why to use Caching ?

Caches are widely used in most of the high volume applications to:

- Reduce Latency
- Increase Capacity
- Improve App Availability

## Four major caching types used in web development :

* ### Web Caching
  * Web Caching helps reduce overall network traffic and latency.
  * Browser caching helps individual users to quickly navigate pages they have recently visited.
  * This process requires Cache-Control and ETag headers to be present to instruct the user’s browser to cache certain files, for a certain period of time.
  * Proxy and Gateway cache allow cached information to be shared across larger groups of users.
  * Data that does not change frequently and can be cached for longer periods of time is cached on Proxy or Gateway servers. E.g.: DNS data that resolve domain names to the IP address.
  
* ### Data Caching
   * Data Caching is very important for DB driven applications.
   * It stores the data in local memory on the server and helps avoid extra trips to the DB for retrieving Data that has not changed.
   * For most DB solutions, cache frequently used queries in order to reduce turnaround time.
   * It is standard practice to clear any cache data after it has been altered.
  
* ### Application Caching
   * While Data Caching storing raw data sets, Application/Output Caching utilizes server-level caching techniques that cache raw HTML.
   * It can be a page or parts of a page (headers/footers), but it is usually HTML markup.
   * This type of caching can drastically reduce website load time and reduce server overhead.

* ### Distributed Caching
   * Distributed cache is typically made up of a cluster of cheaper machines only serving up memory.
   * High volume applications such as Google, YouTube and Amazon use Clustered Distributed Caching.
   *  Once the cluster is setup a new machine of memory can be added at any time without disrupting users.
   *  Allows the web servers to pull and store from distributed server’s memory.
   *  Allows the webserver to simply serve pages and not have to worry about running out of memory.

## Conclusion and further improvements



During a new project, many performance improvements and scalability issues can be solved by proper use of caching. If implemented properly cache can shift load between host and server and the amount of data exchanged between host and server can be reduced considerably and the stability of website/web-app can be ensured even in times of network request failure. Some of the items that remained for further improvements and discussions are Varying responses, Last-Modified, Server load balancing, CDN server caching, etc.

##  References
* [Wikipedia](https://en.wikipedia.org/wiki/Cache_(computing))
* [Medium Artical](https://bootcamp.uxdesign.cc/caching-techniques-one-should-know-603e09d2b298)
* [Fortinet](https://www.fortinet.com/resources/cyberglossary/what-is-caching)
* [Towards Data Science](https://towardsdatascience.com/system-design-basics-getting-started-with-caching-c2c3e934064a)
