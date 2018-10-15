FROM pyfreyr/python:3.6-ubuntu16.04

RUN conda install -y tensorflow-gpu=1.7.0 && \
    conda clean -tipsy

RUN pip install absl-py

ENV NVIDIA_VISIBLE_DEVICES all
ENV NVIDIA_DRIVER_CAPABILITIES compute,utility
ENV NVIDIA_REQUIRE_CUDA "cuda>=9.0"

