# codetocloud-workshop

The application used in this workshop repository is from [WebGoat](https://github.com/WebGoat/WebGoat), an intentionally vulnerable project maintained by OWASP.

## Setup
Open GitHub Codespaces (<> Code -> Codespaces tab -> Create codespace on main)

`mvn clean install`

`./mvnw spring-boot:run`

### Local setup
If you would like to build the code locally follow the setup instructions from [WebGoat](https://github.com/WebGoat/WebGoat#readme).

## Some tips to get you started
We'll be doing more reading of code then writing in this workshop so even if you aren't totally familiar with Java or the Spring framework you can participate.

Here's what you need to know: Spring provides inversion of control (ioc) to Java applications meaning the framework decides the program flow of the application and defines when objects are created and destroyed. This allows developers to spend more time focused on developing business logic. It's a complex system but a couple of key things to know are:
- the Spring container is responsible for managing the beans
- What is a bean you ask? A bean is an instance of a class. You will often see these indicated by annotations like @Component and @Bean throughout the codebase

File structure:
src/main/java/org/owasp/webgoat
    container/ - start looking here for security flaws
        
    lessons/ - include success criteria for each lesson
    server/ - some startup classes, StartWebGoat:main is the application entrypoint
    webwolf/ - a sibling application to Webgoat that simulates an attacker
pom.xml - Maven configuration file that also defines third party dependencies used in Webgoat

## The Fine Print

It is worth noting that this is **NOT SUPPORTED** by Sonatype, and is a contribution of ours
to the open source community (read: you!)

Remember:

* Use this contribution at the risk tolerance that you have
* Do NOT file Sonatype support tickets related to `codetocloud-workshop` support in regard to this project
* DO file issues here on GitHub, so that the community can pitch in

Phew, that was easier than I thought. Last but not least of all:

Have fun creating and using `codetocloud-workshop`, we are glad to have you here!
