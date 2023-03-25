# ConfigServer
 config server is used to define the common and specific properties that is needed for the microservices.

http://localhost:8888/application/default
	response =  {"name":"application","profiles":["default"],"label":null,"version":null,"state":null,"propertySources":[{"name":"file:/E:/config/application.properties","source":{"greeting":"Hello World from Config Server"}}]}
	
http://localhost:8888/config-client/default
	response =  {"name":"config-client","profiles":["default"],"label":null,"version":null,"state":null,"propertySources":[{"name":"file:/E:/config/config-client.properties","source":{"message":"Hello! from Spring Cloud Config Server for Config Client one"}},{"name":"file:/E:/config/application.properties","source":{"greeting":"Hello World from Config Server"}}]}
	
http://localhost:8888/config-client2/default
	response =  {"name":"config-client2","profiles":["default"],"label":null,"version":null,"state":null,"propertySources":[{"name":"file:/E:/config/config-client2.properties","source":{"message":"Hello! from Spring Cloud Config Server for Config Client two"}},{"name":"file:/E:/config/application.properties","source":{"greeting":"Hello World from Config Server"}}]}
	
	
E:/config/config-client2.properties
	message:Hello! from Spring Cloud Config Server for Config Client two
E:/config/config-client.properties
	message:Hello! from Spring Cloud Config Server for Config Client one
E:/config/application.properties
	greeting:Hello World from Config Server
	
