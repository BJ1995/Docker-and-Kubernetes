FROM golang
WORKDIR /web
COPY dispatcher.go .
COPY static/ ./static
RUN go build dispatcher.go
CMD /web/dispatcher
