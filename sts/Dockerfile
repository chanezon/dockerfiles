FROM java:8
MAINTAINER Patrick Chanezon <chanezon@docker.com>

RUN mkdir -p /usr/local/spring && wget -O /usr/local/spring/spring.tar.gz http://dist.springsource.com/release/STS/3.7.3.RELEASE/dist/e4.6/spring-tool-suite-3.7.3.RELEASE-e4.6-linux-gtk-x86_64.tar.gz && gunzip /usr/local/spring/spring.tar.gz && tar -xvf /usr/local/spring/spring.tar -C /usr/local/spring/
RUN mkdir /workspace
VOLUME /workspace
WORKDIR /workspace
CMD ["/usr/local/spring/sts-bundle/sts-3.7.3.RELEASE/STS","-data","/workspace"]
