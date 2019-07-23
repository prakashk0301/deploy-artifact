Download artifact from jenkins dashboard.

wget --auth-no-challenge --http-user=<jenkinsuser> --http-password=<jenkinspassword> http://Jenkins IP:8080/job/ci-job/4/artifact/webapp/target/webapp.war


Create docker image.

docker build -t tomcat1 .



Create docker container.

docker run -itd --name mytomcat1 -p 7002:8080 tomcat1

