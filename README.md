## Spring Boot Multi-Module

### Multi-Module Project:
A Spring Boot project that contains nested maven projects is called the multi-module project. In the multi-module project, the parent project works as a container for base maven configurations.
In other words, a multi-module project is built from a parent pom that manages a group of submodules. Or A multi-module project is defined by a parent POM referencing one or more submodules.
The parent maven project must contain the packaging type pom that makes the project as an aggregator. The pom.xml file of the parent project consists the list of all modules, common dependencies, and properties that are inherited by the child projects. The parent pom is located in the project's root directory. The child modules are actual Spring Boot projects that inherit the maven properties from the parent project.

further references:     
- https://spring.io/guides/gs/multi-module/
- https://www.baeldung.com/spring-boot-multiple-modules
- https://www.javatpoint.com/spring-boot-multi-module-project

### Project Descriptions:
please see application.properties files in resources folder and select a active profile "dev" or "com" to run project. you can check test methods too.  

### IntellliJ IDEA Configurations:
- IntelijIDEA: Help -> Edit Custom Vm Options -> add these two line:
    - -Dfile.encoding=UTF-8
    - -Dconsole.encoding=UTF-8
- IntelijIDEA: File -> Settings -> Editor -> File Encodings-> Project Encoding: form "System default" to UTF-8. May be it affected somehow.
- IntelijIDEA: File -> Settings -> Editor -> General -> Code Completion -> check "show the documentation popup in 500 ms"
- IntelijIDEA: File -> Settings -> Editor -> General -> Auto Import -> check "Optimize imports on the fly (for current project)"
- IntelijIDEA: File -> Settings -> Editor -> Color Scheme -> Color Scheme Font -> Scheme: Default -> uncheck "Show only monospaced fonts" and set font to "Tahoma"
- IntelijIDEA: Run -> Edit Configuration -> Spring Boot -> XXXApplication -> Environment -> VM Options: -Dspring.profiles.active=dev

<hr/>
<a href="mailto:eng.motahari@gmail.com?"><img src="https://img.shields.io/badge/gmail-%23DD0031.svg?&style=for-the-badge&logo=gmail&logoColor=white"/></a>

