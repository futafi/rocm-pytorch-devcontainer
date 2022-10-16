FROM rocm/pytorch:rocm5.3_ubuntu20.04_py3.7_pytorch_1.12.1


ENV HSA_OVERRIDE_GFX_VERSION=9.0.0
RUN apt update -y && \
	apt install -y \
	tig \
	htop \
	curl \
	wget \
	vim

RUN conda install \
	ipykernel 

RUN pip install \
	japanize-matplotlib
