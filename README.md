JRebel plugin for Maven
-----------------------

This plugin is used to generate the **rebel.xml** configuration file for JRebel.

For more information, please refer to the documentation at: **http://manuals.zeroturnaround.com/jrebel/standalone/config.html#maven** 

Usage
-----

Add the following snippet to the **pom.xml** of your Maven project to generate the **rebel.xml** configuration:

```xml
<plugin>
  <groupId>org.zeroturnaround</groupId>
  <artifactId>jrebel-maven-plugin</artifactId>
  <version>1.1.5</version>
  <executions>
    <execution>
      <id>generate-rebel-xml</id>
      <phase>process-resources</phase>
      <goals>
        <goal>generate</goal>
      </goals>
    </execution>
  </executions>
</plugin>
```

To manually execute the goal, run 'mvn jrebel:generate' and rebel.xml will be generated to the target directory. 
