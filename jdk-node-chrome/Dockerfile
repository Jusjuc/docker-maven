FROM docker-io.bvartifactory01.org.nasdaqomx.com/maven:3.6.3-jdk-11

RUN echo $JAVA_HOME
RUN echo $MAVEN_HOME

RUN apt-get update -y
RUN apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates
RUN curl -sL https://deb.nodesource.com/setup_14.x | bash -

# Install Maven and Java
RUN apt-get install -y nodejs

# Install Chrome
RUN wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
RUN dpkg -i google-chrome-stable_current_amd64.deb; apt-get -fy install