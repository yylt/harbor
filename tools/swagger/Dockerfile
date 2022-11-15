FROM golang:1.18.6

ARG SWAGGER_VERSION
RUN curl -x http://172.17.0.1:1080 -fsSL -o /usr/bin/swagger https://github.com/go-swagger/go-swagger/releases/download/$SWAGGER_VERSION/swagger_linux_amd64 && chmod +x /usr/bin/swagger

ENTRYPOINT ["/usr/bin/swagger"]
CMD ["--help"]
