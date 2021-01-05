ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}

RUN elasticsearch-plugin install repository-s3
# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
