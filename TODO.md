# TODO List

## Refactor Project
- Overarching Maven project
- mvn module for library code
- add mvn module for authoritative server as submodule
- add mvn module for basic client as submodule
- mvn module for library classes needed in all parts (DNSMessage, ...)

## Library Code
- make DNSMessage, DNSQuestion, DNSAnswer immutable, only mutate Builders, then build
  - validate bytes when build() is called (OPCode Query matches QR flag, and others)
- allow to transform DNSMessage, DNSQuestion, DNSAnswer to respective Builder too
- get DNSQuestion, DNSAnswer from bytes
- make DNSQuestion


## authoritative server
- in memory database of zones

## implement a client
  - send questions over network
  

### integration test question and question sender
- docker container with question sender
  - integration test: question sender in docker container, send questions to BIND9 Server
  
 

