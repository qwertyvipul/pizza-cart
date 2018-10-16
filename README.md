# pizza-cart

### Reference
![Tech Zambo](https://youtu.be/sB7-ChpjWVw)

### Topics
```markdown
1. Demo Web Application
2. HTTP protocol fundamentals
3. Web Application Architecture
```

### Requirements
```markdown
1. JDK 1.8 & JRE 1.8 - Required for Java (Do not change or remove an
2. Eclipse Mars IDE - IDE for Java Development
3. ![MySQL Installer version 5.6.37](dev.mysql.com/downloads/installer)
4. Maven (Download binary version and unzip in any folder)
```

### Features
```markdown
Admin
1. Login using username and password
2. Can add veg and non-veg pizzas to the inventory
3. Can also upload images of the pizza

Consumer
1. Login using username and password
2. Can browse through the pizzas added in the inventory
3. Add pizzas to the cart and modify the cart
4. Place the order
```

### HTTP
```markdown
1. Request Response Protocol
2. Stateless

3. Http Request contains 2 blocks of information
	* Header
	* Content
	
4. Http Response contains up to 2 blocks of information
	* Completion status information
	* Requested Information
```

### HTTP Request
```markdown
1. GET - Request using GET should only retrieve data
2. HEAD - Similar to GET request, but without the response body. (useful to retrieve meta-information like Google Search).
3. POST - This is to add new data or update existing data

4. PUT - Requests that the enclosed entity be stored under the supplied URI.
	* If the URI refers to an already existing resource, it is modified.
	* If the URI does not point to an existing resource, then the server can create the resource with that URI.

4. DELETE - Deleted the specified resource.
```

**HTTP server are expected to implement GET and HEAD methods at minimum and also the OPTIONS method whenever possible.**

### Difference between POST and PUT
```markdown
POST sends the request to the URI and expects the server to handle the request.
PUT a file or resource at specified URI and only there and create or replace the file or resource at URI.
```

### Web Application Architecture
![Web Applications Architecture](/images/web-application-architecture.png)

### Maven
![Maven Concepts](/images/maven-concepts.png)

### Maven Build Process
```markdown
maven build process is split into 
1. Build Life Cycles - contains sequence of build phases
2. Build Phases - contains sequence of build goals
3. Build Goals
```

### Maven Build Process
![Maven Build Process](/images/maven-build-process.png)

### POM Overview
![POM Overview](/images/pom-overview.png)

### Maven Settings File
![Maven Settings File](/images/maven-settings-file.png)

### Getting Started in Eclipse
```markdown
1. Create your workspace
2. File -> New -> Other -> Maven Project -> Next -> (select maven-archetype-webapp) -> Enter Group Id and Architect Id ->Finish
	* Group Id : com.example
	* Architect Id: pizzashoppingcart

3. Create java folder in src/main folder

4. Create package in java folder
	* package : com.example
	
4. Run -> Run Configurations -> Maven Build -> (Right Click) New Configuration -> Name and Goals
	* Name : pizzashoppingcart-run
	* Goals : org-apache-tomcat.maven:tomcat7-maven-plugin:2.1:run
	
5. Create another configuration to clean and build the project
	* Name : pizzashoppingcart-build
	* Goals : clean install
	* Profiles : jdk1.8
	
6. Run the pizzashoppingcart-build configuration
```

### Servlet Life Cycle
![Servlet Life Cycle](/images/servlet-life-cycle.png)