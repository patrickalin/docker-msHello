FROM java:8u111-jre-alpine
COPY opt /opt/
COPY localtime /etc/localtime
RUN apk add --update bash curl
HEALTHCHECK --interval=60s --timeout=300s --retries=3 CMD curl -f http://localhost:8080/greeting || exit 1
