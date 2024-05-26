FROM rocm/pytorch:rocm6.1.1_ubuntu20.04_py3.9_pytorch_1.13.1


ENV HSA_OVERRIDE_GFX_VERSION=9.0.0
RUN apt update -y && \
	apt install -y \
	tig \
	htop \
	curl \
	wget \
	vim

RUN /opt/conda/bin/pip install --upgrade torch torchvision torchaudio torchao --index-url https://download.pytorch.org/whl/nightly/rocm6.1/
# Failed to install
# torchmetrics torchtext

RUN conda install \
	ipykernel \
	pandas \
	autopep8

RUN /opt/conda/bin/pip install \
	japanize-matplotlib \
	requests \
	gymnasium
