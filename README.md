Hi ![](https://user-images.githubusercontent.com/18350557/176309783-0785949b-9127-417c-8b55-ab5a4333674e.gif) My name is Aleksandr Makalov
==========================================================================================================================================

Golang developer
----------------

In 2020, he began studying golang.

There is experience in writing cli and web services, concurrency, rest api, pgsql, tests, git (github), docker, com. work

Understanding the principles of clean architecture, grpc, graphql, working with cache, queues, logging/monitoring systems as separate services, k8s.

In March 2022 (a few days before the SVO), I started working at a new place, due to a number of circumstances, I had to study the organization scheme of the company's services from scratch, make the final decoupling from foreign cloud service providers. After settling the situation in the infrastructure, work began on repairing/modernizing the old functionality, writing a new one. the infrastructure used

\- yandex cloud

\- linux (ubuntu)

\- docker swarm

\- mariadb

\- postgres

\- redis

\- kafka

\- arangodb

\- clickhouse+otel+fluent+grafana (experimentally for collecting logs, metrics, traces)

\- centrifugo

thinking through the stages of dividing the monolith into microservices, adjusting the application to stateless requirements.

In general, responsibilities for organizing and implementing the full life cycle of the application (planning, design, development, sometimes testing, launch), in addition to collecting feedback from end users.

also a serious problem of memory leak was solved using a profiler, which saved decent financial resources on infrastructure.

in June 2023, I got to develop the "directories" microservice in a logistics service. here I got acquainted with the asynchronous-event architecture based on kafka, got acquainted with graphql in more detail. Within six months, the following was implemented:

\- the planned functionality of the reference microservice;

\- a service for calculating the cost of orders using pre-defined formulas was added to the order microservice (for this, the experience of using google/cel-go libraries was studied, applied and documented).

\- adjustments were made to the main module for calculating the cost of transportation, taking into account the update of the order structure.

\- while there was a probationary period, I "slightly" refactored the code :).

\- during the work, a number of problems were solved on parallel services maintained by the company.

the main part of the service architecture was built on internal self-written libraries.

in the spring of 2025, I began to look for ready-made tools oriented towards the asynchronous-event architecture, found the library github.com/ThreeDotsLabs/watermill. in it I took the implementation of the forwarder idea (forwarding events first to the database, and then to the data bus itself, which increases the fault tolerance of the service). I connected nats jetstream as a data bus. I used gin as a router, because I didn’t bother with adapting it to something more lightweight.

at the moment I’m looking at the tech lead direction. but I still have to work and work in this direction.

*   🌍  I'm based in RU. Blagoveschensk
*   🖥️  See my portfolio at [GitHub](http://github.com/AleksandrMac)
*   ✉️  You can contact me at [makalov.alex@yandex.ru](mailto:makalov.alex@yandex.ru)
*   🧠  I'm currently learning watermill, nats, ai, chatbot
*   👥  I'm looking to collaborate on any project
*   💬  Ask me about construction, finance, psychology, human behavior
