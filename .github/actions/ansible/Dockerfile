FROM ubuntu

RUN apt-get update \ 
    && apt-get install -y python3-pip \ 
    && apt-get clean \ 
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

RUN pip3 install --upgrade ansible ansible-lint paramiko

ENV ANSIBLE_HOST_KEY_CHECKING=False

COPY entrypoint.sh /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]
