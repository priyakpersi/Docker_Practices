

FROM registry.access.redhat.com/ubi9/ubi

#setting Metadata
LABEL maintainer = "Sample Test.. "
LABEL description = "Creating sample dockerfile using ubi9 image.."


RUN yum install -y python39

RUN python3.9 -m pip install micropipenv

WORKDIR /app/

COPY Pipfile Pipfile.lock /app/

RUN micropipenv install --deploy

COPY . /app/

CMD ["echo","Hello World!"]

