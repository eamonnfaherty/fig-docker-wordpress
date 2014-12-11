FROM ubuntu:14.04
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && apt-get install php5 php5-mysql mysql-client-5.6 curl -y
ADD run.sh /run.sh 
RUN chmod 755 /run.sh
EXPOSE 8000
CMD ["/run.sh"]
