FROM ibmcom/datapower:latest

ENV  DATAPOWER_ACCEPT_LICENSE=true \
     DATAPOWER_INTERACTIVE=true      

COPY sourcecode/config /drouter/config
COPY sourcecode/local /drouter/local

USER root
RUN  set-user drouter
USER drouter

EXPOSE 8080