[![Build Status](https://travis-ci.com/UNIZAR-30246-WebEngineering/lab2-big-ws.svg?branch=master)](https://travis-ci.com/UNIZAR-30246-WebEngineering/lab2-big-ws)
# Web Engineering 2020-2021 / Big Web Services
**In this assignment your PR must only modify the `README.md` file**. Please, go to the [Wiki](https://github.com/UNIZAR-30246-WebEngineering/lab2-big-ws/wiki) in order to get the instructions for this assignment.


## Primary goal

`DummyTranslator` should throw a `RuntimeException` rather than return a fake response.
Fix this and protect the testing code against:

- Network failures (e.g. the remote web service is down)
- Remote service failures (e.g. the remote web service throws an exception)

Always use a solution related to web services. It is super easy!

## Secondary goals (:gift:)

Solutions must meet primary goals too. 

Granted:
- [Upgrade to WSDL 2.0 and SOAP 1.2](https://github.com/luisgg98/lab2-big-ws/tree/WSDL2.0_AND_SOAP1.2). Achieving this goal Luis García has learnt that the support promised by Spring Web Services for WSDL 2.0 is deceiving but the support for SOAP 1.2 is ok and can be used as transport independed of the WSDL version used :gift:
- [Re-implement the project with GraphQL](https://github.com/rauljavierre/lab2-big-ws/tree/test). Achieving this goal Raul Javierre has not only learnt GraphQL but also has learnt that testing asynchronous endpoints (the GraphQL implementation used is exposed through an asynchronous controller) must be split in two steps in Spring MVC; in addition, he has learned not to use JSON strings (hard and error prone) and to use JSON objects instead (easy and powerful) :gift:  
- [Re-implement the project with gRPC](https://github.com/saul205/lab2-big-ws/tree/gift). Achieving this goal Saúl Flores has learnt that the similitudes and differences between Protobuf/gRPC and WSDL/SOAP. In addition he has learned to use Protobuf and generate code from Protobuf definitions :gift: 
- [Secure the endpoint WS-Security](https://github.com/jgarciapueyo/lab2-big-ws/tree/test). Achieving this goal Jorge García has learnt in addition concepts such as interceptors and callbacks which are widely used in HTTP-related libraries to add new functionalities.

Proposed:

- Project splits in two (client/server), and the `build.gradle` of the client generates classes from a `wsdl` file retrieved from the server during the build 
- Re-implement the project following [Writing Contract-First Web Services tutorial](https://docs.spring.io/spring-ws/docs/3.0.10.RELEASE/reference/#tutorial)
- Re-implement the project with [Thrift](https://github.com/aatarasoff/spring-thrift-starter)

New ideas will be provided if the gift list gets exhausted.

Manifest your intention first by a PR updating this `README.md` with your goal.
If you desist of your goal, release it by a PR so other fellow can try it. 

|NIA    | User name | Repo | Build Status | What was explored | Review for :gift: | Score
|-------|-----------|------|--------------|-------------------|----------------------|--------
|758906 |[Raul Javierre](https://github.com/rauljavierre)|[rauljavierre/lab2-big-ws](https://github.com/rauljavierre/lab2-big-ws/tree/test)|![Build Status](https://travis-ci.com/rauljavierre/lab2-big-ws.svg)|JUnit, code generation|Re-implement the project with [GraphQL](https://www.graphql-java.com/tutorials/getting-started-with-spring-boot/)| :gift:
|758267 |[Pedro Allué](https://github.com/piter1902)|[piter1902/lab2-big-ws](https://github.com/piter1902/lab2-big-ws/tree/test) |  [![Build Status](https://travis-ci.com/piter1902/lab2-big-ws.svg?branch=test)](https://travis-ci.com/piter1902/lab2-big-ws)    |  JUnit Tests     |                      |
|757153 |[Fran Morés](https://github.com/Fran-sw)|[Fran-sw/lab2-big-ws](https://github.com/Fran-sw/lab2-big-ws/tree/test) |[![Build Status](https://travis-ci.com/Fran-sw/lab2-big-ws.svg)](https://travis-ci.com/Fran-sw/lab2-big-ws)       | Spring exceptions (Runtime and Service), JUnit tests|                      |
|761319 |[Marcos Nuez](https://github.com/Markles01)|[Markles01/lab2-big-ws](https://github.com/Markles01/lab2-big-ws/tree/test) |[![Build Status](https://travis-ci.com/Markles01/lab2-big-ws.svg)](https://travis-ci.com/Markles01/lab2-big-ws)       | JUnit tests, Spring exceptions|                      |
|755769 |[Saúl Flores](https://github.com/saul205)|[saul205/lab2-big-ws](https://github.com/saul205/lab2-big-ws/tree/test)|![Build Status](https://travis-ci.com/saul205/lab2-big-ws.svg?branch=test)|[JUnit Exception Testing](https://github.com/junit-team/junit4/wiki/Exception-testing)| Re-implement the project with [gRPC](https://yidongnan.github.io/grpc-spring-boot-starter/en/) [saul205/lab2-big-ws/gift](https://github.com/saul205/lab2-big-ws/tree/gift) | :gift:
|739202 |[Luis García](https://github.com/luisgg98)|[luisgg98/lab2-big-ws](https://github.com/luisgg98/lab2-big-ws/) |  [![Build Status](https://travis-ci.com/luisgg98/lab2-big-ws.svg)](https://travis-ci.com/luisgg98/lab2-big-ws)    |  Exception Tests  |  [Upgrade to WSDL 2.0 and SOAP 1.2](https://github.com/luisgg98/lab2-big-ws/tree/WSDL2.0_AND_SOAP1.2) | :gift: |  
|756123 |[Rogelio Lacruz](https://github.com/RogorStuff)|[RogorStuff/lab2-big-ws](https://github.com/RogorStuff/lab2-big-ws/tree/test) |[![Build Status](https://travis-ci.org/RogorStuff/lab2-big-ws.svg)](https://travis-ci.org/RogorStuff/lab2-big-ws)    | Spring exceptions, JUnit tests |                      |
|760704 |[Álvaro García](https://github.com/Alvarogd6)|[Alvarogd6/lab2-big-ws](https://github.com/Alvarogd6/lab2-big-ws/tree/test)|![Build Status](https://travis-ci.com/Alvarogd6/lab2-big-ws.svg?branch=test)|JUnit, Spring ws exceptions|    |
|760739 |[Alberto Calvo](https://github.com/AlbertoCalvoRubio)|[AlbertoCalvoRubio/lab2-big-ws](https://github.com/AlbertoCalvoRubio/lab2-big-ws/tree/test)|![Build Status](https://travis-ci.com/AlbertoCalvoRubio/lab2-big-ws.svg?branch=test)|Spring Ws exceptions, Junit|                      |
|766685 |[Enrique Ruiz](https://github.com/TheRealFreeman) | [TheRealFreeman/lab2-big-ws](https://github.com/TheRealFreeman/lab2-big-ws/tree/test) | ![Build Status](https://api.travis-ci.com/TheRealFreeman/lab2-big-ws.svg?branch=test) | JUnit and WSDL description |                      |
|755742 |[Juan José Tambo](https://github.com/jtambo99)|[jtambo99/lab2-big-ws](https://github.com/jtambo99/lab2-big-ws/tree/test)|[![Build Status](https://travis-ci.com/jtambo99/lab2-big-ws.svg?branch=test)](https://travis-ci.com/jtambo99/lab2-big-ws) | JUnit test & Spring exceptions |                         | 
|758325 |[Irene Fumanal](https://github.com/irefu)|[irefu/lab2-big-ws](https://github.com/irefu/lab2-big-ws/tree/test) |  [![Build Status](https://travis-ci.org/irefu/lab2-big-ws.svg?branch=test)](https://travis-ci.org/github/irefu/lab2-big-ws)    |  JUnit Tests and Exception    |                      |
|757755 |[Andrés Otero](https://github.com/andrewknoll)|[andrewknoll/lab2-big-ws](https://github.com/andrewknoll/lab2-big-ws/tree/test) |  [![Build Status](https://travis-ci.com/andrewknoll/lab2-big-ws.svg?branch=test)](https://travis-ci.com/github/andrewknoll/lab2-big-ws)    |  JUnit tests, thrown exceptions (by Spring)    |                      |
|740491 |[José Ignacio Hernández](https://github.com/740491)|[740491/lab2-big-ws](https://github.com/740491/lab2-big-ws/tree/test)| ![Build Status](https://travis-ci.com/740491/lab2-big-ws.svg) | Spring exceptions, testing | | 
|738845 |[Victor Martinez](https://github.com/viriannn)|[viriannn/lab2-big-ws](https://github.com/viriannn/lab2-big-ws/tree/test)|![Build Status](https://travis-ci.com/viriannn/lab2-big-ws.svg?branch=test)| Test and exceptions |                      |
|758803 |[Daniel González](https://github.com/Uncastellum/)|[Uncastellum/lab2-big-ws](https://github.com/Uncastellum/lab2-big-ws/tree/test)|![Build Status](https://travis-ci.com/Uncastellum/lab2-big-ws.svg?branch=test)| JUnit, tests and exceptions |                      |
|739324 |[Elena Morón Vidal](https://github.com/elenamv13/) | [elenamv13/lab2-big-ws](https://github.com/elenamv13/lab2-big-ws/tree/test) | [![Build Status](https://travis-ci.com/elenamv13/lab1-git-race.svg)](https://travis-ci.com/elenamv13/lab1-git-race) | Spring throwing exceptions and Junit exception management  |              |                   |                      |
|758807 |[Jorge García](https://github.com/jgarciapueyo/) | [jgarciapueyo/lab2-big-ws](https://github.com/jgarciapueyo/lab2-big-ws/tree/test) | [![Build Status](https://travis-ci.com/jgarciapueyo/lab2-big-ws.svg?branch=test)](https://travis-ci.com/jgarciapueyo/lab2-big-ws) | Spring WebServices Config, JUnit4 and Spring Test | Secure the endpoint [WS-Security](https://docs.spring.io/spring-ws/docs/3.0.10.RELEASE/reference/#security) | :gift: |
|761754 |[David Alloza](https://github.com/david-AT)|[david-AT/lab2-big-ws](https://github.com/david-AT/lab2-big-ws/tree/test) |[![Build Status](https://travis-ci.com/david-AT/lab2-big-ws.svg?branch=test)](https://travis-ci.com/david-AT/lab2-big-ws)       | Exception Tests|                      |
|758635 |[Daniel Huici Meseguer](https://github.com/Kifixo) | [Kifixo/lab2-big-ws](https://github.com/Kifixo/lab2-big-ws/tree/test) | [![Build Status](https://travis-ci.com/Kifixo/lab2-big-ws.svg?branch=test)](https://travis-ci.com/Kifixo/lab2-big-ws) | Spring exceptions, JUnit4 and Spring Test |                      |
|719974 |[Sergio Martínez](https://github.com/Sergio-Martinez-97) | [Sergio-Martinez-97/lab2-big-ws](https://github.com/Sergio-Martinez-97/lab2-big-ws/tree/test) | [![Build Status](https://travis-ci.com/Sergio-Martinez-97/lab2-big-ws.svg?branch=test)](https://travis-ci.com/Sergio-Martinez-97/lab2-big-ws) | Spring Test and exceptions in Junit | | |
|723883 |[Jorge Turbica](https://github.com/turbica) | [turbica/lab2-big-ws](https://github.com/turbica/lab2-big-ws/tree/test) | [![Build Status](https://travis-ci.com/turbica/lab2-big-ws.svg?branch=test)](https://travis-ci.com/turbica/lab2-big-ws) | JUnit test exceptions | | |
|756308 |[Álvaro Santamaría de la Fuente](https://github.com/SanTa45zgz) | [SanTa45zgz/lab2-big-ws](https://github.com/SanTa45zgz/lab2-big-ws/tree/test) | [![Build Status](https://travis-ci.com/SanTa45zgz/lab2-big-ws.svg?branch=test)](https://travis-ci.com/SanTa45zgz/lab2-big-ws) | Spring Exceptions management and JUnit Tests | | |
|764429 |[Martín Gascón](https://github.com/764429) | [764429/lab2-big-ws](https://github.com/764429/lab2-big-ws/tree/test) | [![Build Status](https://travis-ci.com/764429/lab2-big-ws.svg?branch=test)](https://travis-ci.com/764429/lab2-big-ws) | Spring exceptions, JUnit4 and Spring Test |                      |
|737070 |[José Daniel Barceló Labuena](https://github.com/DaniBarcelo) | [DaniBarcelo/lab2-big-ws](https://github.com/DaniBarcelo/lab2-big-ws/tree/test) | [![Build Status](https://api.travis-ci.com/DaniBarcelo/lab2-big-ws.svg?branch=test)](https://travis-ci.com/DaniBarcelo/lab2-big-ws) | Spring exception on tests and Unit Tests | | |
|738233 |[Sergio Torres](https://github.com/cul3bro) | [cul3bro/lab2-big-ws](https://github.com/cul3bro/lab2-big-ws/tree/test) | [![Build Status](https://api.travis-ci.com/cul3bro/lab2-big-ws.svg?branch=test)](https://travis-ci.com/cul3bro/lab2-big-ws) | JUnit excepcions and tests | | |
|764539 |[Eduardo_Ruiz](https://github.com/eduardoRuizC)|[eduRuizC/lab2-big-ws](https://github.com/eduardoRuizC/lab2-big-ws/tree/test)|![Build Status](https://travis-ci.com/eduardoRuizC/lab2-big-ws.svg?branch=test)| Tests and exceptions |                      |
|737791 |[Alejandro Omist](https://github.com/oumist)|[oumist/lab2-big-ws](https://github.com/oumist/lab2-big-ws/tree/test)|![Build Status](https://travis-ci.com/oumist/lab2-big-ws.svg?branch=test)|JUnit Exception Testing| ||
|740241 |[Sergio Álvarez](https://github.com/sergio-alv)|[sergio-alv/lab2-big-ws](https://github.com/sergio-alv/lab2-big-ws/tree/test)| ![Build Status](https://api.travis-ci.org/sergio-alv/lab2-big-ws.svg?branch=test) | Spring exceptions and testing with JUnit | |
|757715 |[Hayk Kocharyan](https://github.com/hayk99)|[hayk99/lab2-big-ws](https://github.com/hayk99/lab2-big-ws/tree/test) |  [![Build Status](https://travis-ci.org/hayk99/lab2-big-ws.svg?branch=test)](https://travis-ci.org/github/hayk99/lab2-big-ws)    |  Added 2 new tests and Spring Exception    |                      |
|735041 |[Eduardo Díaz](https://github.com/ediazl) | [ediazl/lab2-big-ws](https://github.com/ediazl/lab2-big-ws/tree/test) | [![Build Status](https://travis-ci.com/ediazl/lab2-big-ws.svg?branch=test)](https://travis-ci.com/ediazl/lab2-big-ws) | Spring exceptions and Junit tests | | |
|738737 |[Victor Jarreta](https://github.com/VJarreta)|[VJarreta/lab2-big-ws](https://github.com/VJarreta/lab2-big-ws/tree/test) |  [![Build Status](https://travis-ci.com/VJarreta/lab2-big-ws.svg?branch=master)](https://travis-ci.com/github/VJarreta/lab2-big-ws)    |  Tests and exception   |                      |
