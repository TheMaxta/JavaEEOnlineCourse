# Build
mvn clean package && docker build -t academy.learnprogramming/Hello-javaee8 .

# RUN

docker rm -f Hello-javaee8 || true && docker run -d -p 8080:8080 -p 4848:4848 --name Hello-javaee8 academy.learnprogramming/Hello-javaee8 