FROM nginx
LABEL description="httpd image"
LABEL version="1.0"
LABEL fechacreacion="073020"

# RUN apt-get update && apt-get install -y figlet

# RUN mkdir -p /tmp/testing/ && cd /tmp/testing/ && touch test1

COPY index.html /usr/share/nginx/html/

#VOLUME . /devops/www5/
VOLUME /devops/www5

EXPOSE 8080

# docker run -v /home/vagrant/www3/index.html:/usr/share/nginx/html/index.html -p 8282:80 -d nginx