FROM golang:1.18

RUN mkdir ../home/app 
WORKDIR /../home/app
COPY . .
#RUN unset GOPATH

#RUN apt-get update && \
#    ./docker.sh && \
#    rm -rf go.mod && \
#    make install
RUN ./docker.sh && \
    make install
EXPOSE 8080
CMD ["make", "serve"]


