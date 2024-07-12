# Arguments to pass to the image
ARG VERSION_DATE=24.06
ARG FROM_IMAGE=nvcr.io/nvidia/pytorch

# Import RAPIDS container as the BASE Image (cuda base image)
FROM ${FROM_IMAGE}:${VERSION_DATE}-py3
LABEL maintainer="glenn.s.tamkin@nasa.gov" 

ENV TFC_VERSION=0.1.1
ENV VHR_CLOUDMASK_VERSION=main

RUN pip install hydra-core

RUN pip install git+https://github.com/dshean/pygeotools.git@master \
        git+https://github.com/nasa-nccs-hpda/super-resolution-sst.git@main

HEALTHCHECK NONE
ENTRYPOINT [""]
