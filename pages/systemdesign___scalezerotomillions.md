- ((63794612-269f-4ca0-bb69-50ed933acdcd))
  collapsed:: true
	- web app, database, cache etc... in one server
	  ((637946af-b6f6-4d56-aa77-013dd4fc902c))
	- How single server work?
		- 1. User > DNS(Domain Name System) is paid service provided by 3rd parites
		- 2. DNS > IP (Internet Protocol) > User
		- 3. User > HTTP(Hypertext Transfer Protocol) > web server
		- 4. Web server > HTML pages or JSON > User
	- Web traffic
		- Client
		  * client-side languages (HTML,JS)
		  * presentation
		- Server
		  * server-side languages (JAVA, Python etc..)
		  * Handle business logic, storage etc..
	- Mobile to Web server traffic
	  * Communication Protocol: HTTP
	  * JSON(JavaScript Object Notation) for API response
	  * JSON is simple
- ((63794b3e-542c-4971-aa58-47607d328ed0))
  collapsed:: true
	- ((63794f0b-476b-411d-9594-994dafea70de))
	- Relational Database Management System
	  (RDBMS/SQL database)
		- why RDBMS?
		  * used over 40 years old and work well.
		  * Can use join operations using SQL different database tables
		  * RDBMS store in tables and rows
		- RDBMS's languages
		  * MySQL, Oracle Database, PostgreSQL,etc.
	- Non-Relational (NoSQL databases)
		- why NoSQL?
		  * Your application requires super-low latency.
		  * Your data are unstructured, or you do not have any relational data.
		  * You only need to serialize and deserialize data (JSON, XML, YAML, etc.).
		  * You need to store a massive amount of data
		  * join doesn't work in non-RDBMS
		- NoSQL's languages
		  * CouchDB, Neo4j, Cassandra, HBase, Amazon DynamoDB
		- NoSQL's dabase group 4 categories
		  * key-value stores
		  * graph stores
		  * column stores
		  * document store
- ((63794f26-d984-4a03-a114-0ebe80ce6d45))
  collapsed:: true
	- Vertical scaling or scale up
		- Vertical scale - advantages
		  * add more (CPU, RAM etc..) to servers
		  * good when low traffic
		- Vertical scale - disavantages
		  * impossible to add more CPU and memory to one server only
		  * no fail over and redundancy (if one server fail everything fail)
	- Horizontal or scale out
		- Horizontal advantages - 
		  * large scale applications
		  * add more servers to pool of resources
		  * load balancer for handling traffic
		  * independent scaling
		- Horizontal disavantages - 
		  * no direct access to web server
- ((6379518e-15c4-4546-96e8-0f504f10081a))
  collapsed:: true
	- Load balancer evenly distributes incoming traffic among web servers.
	  ((637951e0-ccf8-4fad-bfa2-37b56af53019))
	- Load balancer for Web tier-Advantages
	  * Client access public IP of load balancer
	  * Better security because no more client direct access to Web server
	  * Private IP user for communication between servers with read only
	  * If one server fail the traffic route automatically switch to different server
	  * If traffic over load then load balancer handle it gracefully by adding more servers
- ((63795db8-2f7d-4dce-a46d-95f17f74b0fa))
  collapsed:: true
	- Database replication used for *redundancy and fail over*
	  ((63795dc9-ad18-4142-89d8-05c6813bbeb6))
	- where to use database replications?
	  * can be use many database management systems like master/slave relationship.
	  * master support only **write** operations.
	  * slave database get copies of data from master and read operations.
	  * Data modifying command - insert, delete, or update send to master.
	  * more slaves than master because most app need to read than write
	- Advantages of database replication
	  * Better performance: writes and updates for master nodes; 
	  read for slave nodes. it allows more queries to be processed in parallel.
	  * Reliability: Data is still preserved, if one server destroyed because data is replicated to multiple locations.
	  * High availability: Because of data replication we can still access to datas.
	- If a slave database failed?
	  * Read operation is assigned to Master for temporary if extra slave not available
	  * If extra slave available then old database is copied to new slave and read operation is assigned
	- If a master database failed?
	  * a random slave will become a master for temporary
	  * all master operation will be assigned to a new master
	  * missing data must be up to date for a new master by running data recovery scripts.
	  * replication methods: multi-masters, circular replication etc..
- ((63796475-8b57-46d0-ab59-3efeb3c6ca01))
  collapsed:: true
	- **cache** - is a temporary storage area that stores the result of expensive responses or frequently accessed data in memory so that subsequent requests are served more quickly.
	- ((638ccb4e-3b02-4423-ba34-ed509bfdf26b))
	- **cache tier** -
	  * better system performance
	  * ability to reduce database workloads
	  * the ability to scale the cache tier independently
	- How cache is used?
		- read-through cache -
		  * checks if the cache has the available response. 
		  * If it has, it sends data back to the client. 
		  * If not, it queries the database, stores the response in cache, and sends it back to the client.
	- Why use cache?
		- Data is read frequently but modified infrequently.
		  * Cache is store in volatile memory.
		  * Expiration policy - expiration should not be too short or too long. 
		  * Consistency - data store and cache  must be in sync
		- Mitigating failures - 
		  Single Point Of Failure (SPOF) can be mitigate with cache servers different data centers.
		  * Eviction Policy - removed pre-existing data if cache is full. 
		  * Eviction Methods -  
		  Least-recently-used(LRU)
		  First in First Out (FIFO)
		-
- ((638cd160-0923-46b8-b6ed-4f5da5089977))
  collapsed:: true
	- CDN - static content like images, videos, CSS, JavaScript files, etc..
	- Dynamic content caching - 
	  * new concept
	  * enables the caching of HTML pages that are based on request path, 
	  * query strings, cookies, and request header.
	- ((638ce61e-6d75-4dd8-b3ce-ff753df0bab1))
	- ((638ce64f-ba44-417e-8cfb-9460e92e59ce))
	- Why use CDN?
		- * Cost
		  * Setting an appropriate cache expiry
		  * CDN fallback
		  * Invalidating files
	- CDN and cache added design
		- ((638ce7e0-eea8-4079-82ef-6d1fbd30ff89))
- ((638ce800-bc22-4593-84dd-267316e75c6a))
  collapsed:: true
	- scaling web tier in horizontally - move session data the persistent storage
	  * relational database or NoSQL
	- stateful architecture - 
	  * A stateful server remembers client data (state) from one request to the next
	  * ((638cfd92-2d6e-4ff3-9d82-b6a82de0937b))
	  * routing same server can be done with sticky session in most balancers
	  * but adds overhead.
	  * also not good for handle server failures.
	- state less - server keeps no state information.
	  * which fetch state data from a shared data store. 
	  * State data is stored in a shared data store and kept out of web servers.
	- ((638cfe91-53ed-49ef-9949-02a281ea5eaf))
	- improve availability and 
	  * provide a better user experience across wider geographical areas,
	  * supporting multiple data centers is crucial.
- ((638cff33-b0f4-4455-82fa-ed1bfa9fed4f))
	-