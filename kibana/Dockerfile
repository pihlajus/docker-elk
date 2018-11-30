ARG ELK_VERSION

# https://github.com/elastic/kibana-docker
FROM docker.elastic.co/kibana/kibana-oss:${ELK_VERSION}

# Add your kibana plugins setup here
RUN kibana-plugin install https://github.com/sivasamyk/logtrail/releases/download/v0.1.30/logtrail-6.5.0-0.1.30.zip
COPY config/logtrail.json plugins/logtrail/
