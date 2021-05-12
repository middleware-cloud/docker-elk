ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu


ARG ELK_VERSION

RUN sh -c '/bin/echo -e "y" | elasticsearch-plugin install https://github.com/medcl/elasticsearch-analysis-ik/releases/download/v${ELK_VERSION}/elasticsearch-analysis-ik-${ELK_VERSION}.zip'

