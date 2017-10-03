# JPASchemaGeneration
```xml
<?xml version="1.0" encoding="UTF-8"?>
<persistence version="2.1" xmlns="http://xmlns.jcp.org/xml/ns/persistence" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/persistence http://xmlns.jcp.org/xml/ns/persistence/persistence_2_1.xsd">
  <persistence-unit name="JPASchemaGeneration" transaction-type="JTA">
    <jta-data-source>jdbc/localpg</jta-data-source>
    <class>com.ilkinabdullayev.jpaschemageneration.Employee</class>
    <exclude-unlisted-classes>true</exclude-unlisted-classes>
    <properties>
      <property name="javax.persistence.schema-generation.scripts.action" value="drop-and-create"/>
      <property name="javax.persistence.schema-generation.database.action" value="drop-and-create"/>
      <property name="javax.persistence.schema-generation.create-source" value="script"/>
      <property name="javax.persistence.schema-generation.drop-source" value="script"/>
      <property name="javax.persistence.schema-generation.create-script-source" value="META-INF/create.sql"/>
      <property name="javax.persistence.schema-generation.drop-script-source" value="META-INF/drop.sql"/>
      <property name="javax.persistence.sql-load-script-source" value="META-INF/load.sql"/>
      <property name="javax.persistence.schema-generation.scripts.create-target" value="file:/Users/ilkinabdullayev/Documents/test2/create.sql"/>
      <property name="javax.persistence.schema-generation.scripts.drop-target" value="file:/Users/ilkinabdullayev/Documents/test2/drop.sql"/>
      <property name="eclipselink.logging.level" value="FINE"/>
    </properties>
  </persistence-unit>
</persistence>
```
