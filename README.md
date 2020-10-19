[![Build Status](https://travis-ci.com/UNIZAR-30246-WebEngineering/lab2-big-ws.svg?branch=master)](https://travis-ci.com/UNIZAR-30246-WebEngineering/lab2-big-ws)
# Web Engineering 2020-2021 / Big Web Services
Please, go to the [Wiki](https://github.com/UNIZAR-30246-WebEngineering/lab2-big-ws/wiki) in order to get the instructions for this assignment.

## Primary goal

`DummyTranslator` should throw a `RuntimeException` rather than return a fake response.
Fix this and protect the testing code against:

- Network failures (e.g. the remote web service is down)
- Remote service failures (e.g. the remote web service throws an exception)

Always use a solution related to web services. It is super easy!

## Secondary goals (:gift:)

Solutions must meet primary goals too. 

- Upgrade to WSDL 2.0 and SOAP 1.2
- Secure the endpoint [WS-Security](https://docs.spring.io/spring-ws/docs/3.0.10.RELEASE/reference/#security)
- Project splits in two (client/server), and the `build.gradle` of the client generates classes from a `wsdl` file retrieved from the server during the build 
- Re-implement the project following [Writing Contract-First Web Services tutorial](https://docs.spring.io/spring-ws/docs/3.0.10.RELEASE/reference/#tutorial)
- Re-implement the project with [gRPC](https://yidongnan.github.io/grpc-spring-boot-starter/en/)
- Re-implement the project with [GraphQL](https://www.graphql-java.com/tutorials/getting-started-with-spring-boot/)
- Re-implement the project with [Thrift](https://github.com/aatarasoff/spring-thrift-starter)

New ideas will be provided if the gift list gets exhausted.

Manifest your intention first by a PR updating this `README.md` with your goal.
If you desist of your goal, release it by a PR so other fellow can try it. 

|NIA    | User name | Repo | Build Status | What was explored | Review for :gift: | Score
|-------|-----------|------|--------------|-------------------|----------------------|--------
| 757153|   Fran-sw |      |[![Build Status](https://travis-ci.com/Fran-sw/lab2-big-ws.svg)](https://travis-ci.com/Fran-sw/lab2-big-ws)       |                   |                      |

