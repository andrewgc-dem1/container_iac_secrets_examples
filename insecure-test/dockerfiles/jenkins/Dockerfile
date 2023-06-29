FROM juliantotzek/jenkins-maven
# if we want to install via apt
USER root
RUN apt-get update && apt-get install -y maven docker
# USER jenkins # drop back to the regular jenkins user - good practice

