# HeroesAPI
Gerenciamento de Super Heróis da Marvel e da DC
API reativa com Spring Boot | Digital Innovation One
Web project using a hero management API with Spring WebFlux, employed by companies like Netflix and Pivotal, along with the Reactor reactive library that is currently maintained by VmWare.

📌 Index
⚙ Settings
💻 Technologies
🚀 How to run
⚙ Settings
Have a AWS Command Line Interface, set up following the steps. For more details watch the video.

💻 Technologies
- Java
- Spring Boot
- WebFlux (working reactively in spring and Netty embedded server)
- AWS DynamoDB (fully managed proprietary NoSQL database service that supports key-value and document data structures)
- JUnit
- SLF4J (The Simple Logging Facade for Java serves as a simple facade or abstraction for various logging frameworks (e.g. java.util.logging, logback, log4j) allowing the end user to plug in the desired logging framework at deployment time)
- Project Reactor ( fourth-generation reactive library, based on the Reactive Streams specification, for building non-blocking applications on the JVM)
🚀 How to run
Cloning the repository

  # Cloning repository
  git clone https://github.com/antoniosergiojr/heroesApi_digital_innovation_one.git
Running web project

  # Accessing web project
  cd heroesApi_digital_innovation_one

  # Running web project
  Run dynamo (AWS Command Line Interface): 

  aws configure (insert key ID, Access Key and Region us-east-1)

  java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb

  aws dynamodb list-tables --endpoint-url http://localhost:8000

  swagger: http://localhost:8080/swagger-ui-heroes-reactive-api.html
