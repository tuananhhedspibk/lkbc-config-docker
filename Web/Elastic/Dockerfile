FROM elasticsearch:5.3.1

MAINTAINER lkbc.team@gmail.com

COPY elasticsearch-analysis-vietnamese-5.3.1.zip /usr/share/elasticsearch/

RUN cd /usr/share/elasticsearch && \
  bin/elasticsearch-plugin install file:///usr/share/elasticsearch/elasticsearch-analysis-vietnamese-5.3.1.zip && \
  bin/elasticsearch-plugin install analysis-icu