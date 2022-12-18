FROM golang:1.18

RUN mkdir ../home/app 
WORKDIR /../home/app
COPY . .
RUN ./req.sh
EXPOSE 8080
CMD ["go", "run", "main.go"]
