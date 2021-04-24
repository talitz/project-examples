# Environment integration Java8 + nginx
FROM docker.bintray.io/jfrog/pipelines-u18java:8
#ENV BUILD_NUMBER
# get the jar
RUN apt-get update

COPY gradle_results/com/jfrog/frogsws/*/*.jar /ws/frogsws.jar
COPY wrapper.sh /wrapper.sh

EXPOSE 81 9000

CMD ["/wrapper.sh"]
