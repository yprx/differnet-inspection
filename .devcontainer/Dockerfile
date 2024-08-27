FROM tensorflow/tensorflow:latest-gpu

WORKDIR /workspaces/differnet-inspection

RUN apt update && \
    DEBIAN_FRONTEND=noninteractive apt install -y software-properties-common && \
    apt install -y python3-apt && \
    apt install -y libgl1 && \
    apt install -y jq curl && \
    apt install -y git && \
    apt install -y python3-pip

RUN update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.10 1
RUN update-alternatives --install /usr/bin/python python /usr/bin/python3.10 1

RUN add-apt-repository ppa:deadsnakes/ppa && apt update
RUN apt install -y python3.10

