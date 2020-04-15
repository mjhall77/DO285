FROM ubi7/ubi:7.7

MAINTAINER mjhall77

LABEL description="A cusomt Apache container based on UBI 7"

RUN yum install -y httpd && yum clean all -y

RUN echo "Hello from Dockerfie" > /usr/share/httpd/noindex/index.html

EXPOSE 80

ENTRYPOINT ["httpd", "-D", "FOREGROUND"]
