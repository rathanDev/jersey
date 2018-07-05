reference:
https://jersey.github.io/documentation/latest/getting-started.html#new-from-archetype

mvn archetype:generate -DarchetypeArtifactId=jersey-quickstart-grizzly2 \
-DarchetypeGroupId=org.glassfish.jersey.archetypes -DinteractiveMode=false \
-DgroupId=com.example -DartifactId=simple-service -Dpackage=com.example \
-DarchetypeVersion=2.27

mvn clean test

to check it in browser
http://localhost:8080/myapp/myresource

or
curl http://localhost:8080/myapp/myresource

To run it in stand alone mode
mvn exec:java

