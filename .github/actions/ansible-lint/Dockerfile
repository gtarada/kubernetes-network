FROM ubuntu

RUN apt update && apt install python3-pip

RUN pip3 install --upgrade ansible ansible-lint paramiko

ENV ANSIBLE_HOST_KEY_CHECKING=False

ENTRYPOINT ["/bin/sh", "-c"]
