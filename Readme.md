## Types of communication
    1. Synchronous (Strong coupling)
    2. HTTP (REST/GraphQL)
    3. Websocket (debatable if sync or async)
 
## Asynchronous (Weak coupling)
    1.Messaging queues
    2.Pub subs
    3.Server-Sent Events 
    4.Websocket (debatable if sync or async)
 ## Scaling ws servers
    In the real world, you’d want more than one websocket servers         (Especially as your website gets more traffic)
    The way to scale websocket servers usually happens by creating a ws fleet
    There is usually a central layer behind it that orchestrates  messages
    ws servers are kept stateless

## Commands for Message Queue and Pub Sub Architecture and Redis
    - snapshots to be used to recover the in memory data provided by the Redis cache
    - Let’s start redis locally and start using it as a DB
        - docker run --name my-redis -d -p 6379:6379 redis
    - Connecting to your container
        - docker exec -it container_id /bin/bash
    - Connecting to the redis cli
        - redis-cli
