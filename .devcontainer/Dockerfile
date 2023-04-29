FROM rocm/pytorch:rocm5.4.3_ubuntu20.04_py3.8_pytorch_1.10.1


ENV HSA_OVERRIDE_GFX_VERSION=9.0.0
RUN apt update -y && \
	apt install -y \
	tig \
	htop \
	curl \
	wget \
	vim

RUN /opt/conda/bin/pip install --upgrade --force-reinstall torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm5.4.2

RUN conda install \
	ipykernel \
	pandas \
	autopep8

RUN /opt/conda/bin/pip install \
	japanize-matplotlib \
	requests \
	gymnasium
