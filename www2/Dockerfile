FROM nginx:latest
LABEL description="Page docker file"
LABEL version=1.0
LABEL fechacreacion=072820

# RUN apt-get update && apt-get install -y figlet

# RUN mkdir -p /tmp/testing/ && cd /tmp/testing/ && touch test1

COPY index.html /usr/share/nginx/html/

# docker run -v /home/vagrant/www3/index.html:/usr/share/nginx/html/index.html -p 8282:80 -d nginx