# standard-maven-pom.github.io

Maven `pom.xml` is to be treated as code. Using [POM Reference](http://maven.apache.org/pom.html)
the order of element as follows:

```
  <!-- Main POM entries -->
  <parent>...</parent> optional

  <groupId>...</groupId>
  <artifactId>...</artifactId>
  <version>...</version>
  <packaging>...</packaging>

  <properties>...</properties>

  
  for pom modules
  <modules>...</modules>
  <dependencyManagement>...</dependencyManagement>
  
  for jar modules
  <dependencies>...</dependencies>
 ``` 

Recommended dependencies order (blocks are separated by empty line):
- current project dependencies, i.e. other modules
- internal other departments 
- main framework dependencies, e.g. `spring`
- standard dependencies
- less often used dependencies

---

This mini-site is created by
Paul Verest.
2021
