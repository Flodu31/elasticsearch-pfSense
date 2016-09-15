FROM logstash:latest

# Download GeoIP Data
RUN mkdir -p /usr/share/GeoIP/ && \
   curl "http://geolite.maxmind.com/download/geoip/database/GeoLiteCity.dat.gz" >> /usr/share/GeoIP/GeoLiteCity.dat.gz && \
   gunzip /usr/share/GeoIP/GeoLiteCity.dat.gz && \
   mkdir /etc/logstash/conf.d/patterns/

COPY config/logstash.conf /etc/logstash/conf.d/
COPY config/pfsense2-2.grok /etc/logstash/conf.d/patterns/

#docker start cf6b6ceb1aca
#docker exec -t -i cf6b6ceb1aca /bin/bash
#cd /etc/logstash/conf.d/
#mkdir patterns
#docker cp logstash.conf cf6b6ceb1aca:/etc/logstash/conf.d/
#docker cp pfsense2-2.grok cf6b6ceb1aca:/etc/logstash/conf.d/patterns/