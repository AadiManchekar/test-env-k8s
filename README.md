# test-env-k8s
Large Enterprises use a k8s test environment to do their testing be it on dev level or QA level. 
repo contains basic boilerplate code that will help u get started with Creating your own test-environment for your enterprise :)

## Infra Components
To create an ideal test environment, you must have infra components to be up always. We cannot run them as pods since pods may be rescheduled or they might be stuck in containercreating/ Not Ready state due to a lack of resources. We cannot afford this, hence we must operate some core infra components as Docker containers. You can have them on a dedicated node. Make sure that node has a taint so that no other pods schedule on it. 

Some Core infra components can be:

 1. Kafka/RabbitMQ
 2. Nginx (Serve https/gRPC/wss requests)
 3. Postgresql/Mysql (To store SQL data)
 4. neo4j (GraphDB)
 5. Cassandra (To store No SQL data)
 6. Spark (if you are processing some data)

    enter code here

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTg0NTgwMzI4LC03OTQzMzU5OTksMTcyOT
Q5Mjk2NSwtMTcyMDA3MDg2NF19
-->