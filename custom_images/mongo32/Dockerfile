FROM mongo:3.2.10

MAINTAINER devops@gsa.gov

RUN apt-get update
RUN apt-get -y install netcat

COPY scripts /scripts
RUN chmod +x /scripts/*.sh
RUN touch /.firstrun

ENTRYPOINT ["/scripts/run.sh"]
CMD [""]
