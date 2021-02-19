ARG UPSTREAM_VERSION
FROM  shahanafarooqui/rtl:$UPSTREAM_VERSION

### NO ENTRYPOINT
#COPY ./RTL-Config.json /RTL

### WITH ENTRYPOINT
COPY ./entrypoint.sh /RTL
RUN chmod +x entrypoint.sh
ENTRYPOINT ["/sbin/tini", "-g", "--", "/RTL/entrypoint.sh"]
