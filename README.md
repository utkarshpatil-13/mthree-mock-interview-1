# mthree-mock-interview-1
Mthree Mock interview

Difference between ConcurrentHashMap and HashMap
- hashmap is not synchronized, concurrent hashmap is synchronized
- hashmap is not thread safe, concurrenthashmap is not thread safe
- so let's say we are using a banking application and we are updating the account balance of let's say a person. If there are two transactions that are updating the account balance of that person, it might happen that incorrect balance may be shown because of non-synchronization with the use of hashmap, so for that we can use concurrent hashmap

Design a transaction system of banking application
- in a banking application, I will first make the use of @Transactional annotation to maintain the atomicity of the application.
- also I will make sure to use the caching techniques effectively so that I can maintain consistency between cache and db.
- for isolation I will use thread safe elements into my application so that no transaction and enter and modify the working of another transaction
- for durability I will use cloud storage for my dbms like aws, gcp, etc. so that it will remain available in every scenario

How do you handle authentication and authentication in spring boot and react
- For authorization and authentication, there are various things that we can do like - jwt auth, outh2client, multi-factor auth, etc
- In spring boot - spring security is the library which is used to build the authentication and authorization part.
- Flow of authentication (jwt case):
-   - when a user hits an api for login, if I found the user registered into the db, I will return him a jwt token which he can use for navigating into the application.
