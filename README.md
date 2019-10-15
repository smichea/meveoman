# Meveoman

Meveoman is a Meveo script that be also used as a standalone java app to execute a Postman 2.1 collection.

## Usage

### As a standalone java app

1. clone the repo
2. use maven to build (you can easily complie from intelIJ idea)
3. execute the jar meveoman.jar (containing the class org.meveo.postman.PostmanRunnerScript)  
usage : java -jar meveoman.jar <collectionFilename> <environmentFilename>[trustAllCertificates]  
  <collectionFilename>: filename (including path) of the postman 2.1 collection json file.  
  <environmentFilename>: filename (including path) the postmane environment json file to load and initialize the context.  
  trustAllCertificates: if this param is set then ssl certificates are not checked.  

### As a meveo script

1. install and run meveo
2. log in meveo admin console and create a Script "org.meveo.postman.PostmanRunnerScript" and copy the content of the class in it.
3. Use this script through ScriptingJob or Rest Enpoint,...