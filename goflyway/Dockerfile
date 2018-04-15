FROM centos
#RUN apk add --update git go
RUN ["/usr/bin/yum", "-y", "update"]
RUN ["/usr/bin/yum", "-y", "install", "git"]
RUN ["/usr/bin/yum", "-y", "install", "go"]

WORKDIR /
RUN git clone https://github.com/coyove/goflyway.git
WORKDIR /goflyway
ENTRYPOINT ["go", "run", "main.go", "-k=heaven"]
