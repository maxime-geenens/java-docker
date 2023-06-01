# java-docker

### Build & Run with Dockerfile

##### Build
<code>
docker build -f Dockerfile -t my-api-maven .
<code/>

##### Run 
<code>
docker run -p 9010:8080 -it --rm my-api-maven
<code/>