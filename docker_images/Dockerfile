

FROM registry.access.redhat.com/ubi9/ubi

#setting Metadata
LABEL maintainer = "Sample Test.. "
LABEL description = "Creating sample dockerfile using ubi9 image.."


RUN yum install -y git

COPY . /app

WORKDIR /app

EXPOSE 8080

CMD ["echo","Hello World!"]

