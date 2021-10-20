FROM ubuntu
LABEL mantainer="Marcelo Canhamero"
RUN apt-get update && \
    apt-get install -y nginx && \
    rm -rf /var/lib/apt/lists/*
RUN echo "<h1>Curso Docker</h1>" | \
    tee /var/www/html/index.html
VOLUME ["/var/cache/nginx"]
EXPOSE 80 443
CMD ["nginx","-g","daemon off;"]

