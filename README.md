# standard maven pom.xml file order and style

Maven `pom.xml` is to be treated as code. 
Using [POM Reference](http://maven.apache.org/pom.html)
the order of element as follows:

```
  <!-- Main POM entries -->
  <parent>... <!-- optional parent GAV section -->
  </parent>
  
  <groupId>...</groupId>
  <artifactId>...</artifactId>
  <version>...</version>
  <packaging>...</packaging> <!-- if jar, just delete as it is default -->

  <properties>...</properties>
  
  for pom modules
  <modules>...</modules>
  <dependencyManagement>...</dependencyManagement>
  
  for jar modules
  <dependencies>...</dependencies>
 ``` 

Recommended dependencies order (blocks are separated by empty line):
- other modules as dependencies 
- internal other departments 
- main framework dependencies, e.g. `spring`
- usual dependencies
- less often used dependencies
- test scope dependencies

---

This mini-site is created by
Paul Verest.
2021
