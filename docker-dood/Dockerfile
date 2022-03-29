FROM jenkins/jenkins:latest-jdk11

USER root

COPY install_docker.sh /install_docker.sh
RUN chmod +x /install_docker.sh
RUN /install_docker.sh

COPY install_node.sh /install_node.sh
RUN chmod +x /install_node.sh
RUN /install_node.sh

RUN usermod -aG docker jenkins
USER jenkins