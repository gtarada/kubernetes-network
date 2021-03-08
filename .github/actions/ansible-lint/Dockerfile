FROM ubuntu

RUN apt-get update && apt-get install -y python3-pip && rm -rf /var/lib/apt/lists/*

RUN pip3 install --upgrade ansible ansible-lint paramiko

ENV ANSIBLE_HOST_KEY_CHECKING=False

ENTRYPOINT ["/bin/sh", "-c"]
