# Enable liquibase command tool

1. http://www.liquibase.org/
2. Add liquibase path to system (PATH) / # liquibase <arguments>
3. java -jar /e/tools/liquibasedir/liquibase.jar <arguments>

# Command line require arguments arguments

1. --changeLogFile : change log file path
2. --username : database user name
3. --password : database user password
4. --driver : databse JDBC driver
5. --url : the database JDBC url

# Some driver list

1. com.mysql.jdbc.Driver
2. oracle.jdbc.OracleDriver

# Addind JDBC classpath 

1. --classpath : JDBC classpath

## Launch real example over windows using mysql

Create a liquibase.properties in a migration directory. In this case we are using in windows :
DIR : E:/github/liquibase-examples/mysql

[mysql connector]: https://dev.mysql.com/downloads/connector/j/5.0.html
[liquibase properties information]: http://www.liquibase.org/documentation/liquibase.properties.html

### Execute the command passing changelog file

#### Creating first update using a xml changelog file
```

> liquibase --changeLogFile=E:/github/liquibase-examples/mysql/xml/changelog.xml update

```