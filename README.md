```bash
# PHP 5.3
cd php5.3 && docker build -t="meetup/php53" ./
docker run meetup/php53 /usr/bin/php --version

# PHP 5.4
cd php5.4 && docker build -t="meetup/php54" ./
docker run meetup/php54 /usr/bin/php --version

# PHP 5.5
cd php5.5 && docker build -t="meetup/php55" ./
docker run meetup/php55 /usr/bin/php --version

# HHVM
cd hhvm && docker build -t="meetup/hhtm" ./
docker run meetup/hhvm hhvm --version

# Elasticsearch 1.0
cd elasticsearch && docker build -t="meetup/elasticsearch" ./
docker run -d -p 9200:9200 -p 9300:9300 meetup/elasticsearch

wait 10
wget http://localhost:9200
```
