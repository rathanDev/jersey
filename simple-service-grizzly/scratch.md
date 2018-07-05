reference:
https://jersey.github.io/documentation/latest/getting-started.html#new-from-archetype

mvn archetype:generate -DarchetypeArtifactId=jersey-quickstart-grizzly2 \
-DarchetypeGroupId=org.glassfish.jersey.archetypes -DinteractiveMode=false \
-DgroupId=org.jana -DartifactId=simple-service-grizzly -Dpackage=org.jana \
-DarchetypeVersion=2.27

mvn clean test

to check it in browser
http://localhost:8080/myapp/myresource

or
curl http://localhost:8080/myapp/myresource
curl -i http://localhost:8080/myapp/myresource
curl -v http://localhost:8080/myapp/myresource

To run it in stand alone mode
mvn exec:java

