# Arguments to pass to the image
ARG VERSION_DATE=24.06
ARG FROM_IMAGE=nvcr.io/nvidia/pytorch

# Import RAPIDS container as the BASE Image (cuda base image)
FROM ${FROM_IMAGE}:${VERSION_DATE}-py3
LABEL maintainer="glenn.s.tamkin@nasa.gov" 

ENV TFC_VERSION=0.1.1
ENV VHR_CLOUDMASK_VERSION=main

RUN pip install xarrayRUN pip install 
RUN pip install h5netcdf
RUN pip install netCDF4
RUN pip install pydap
RUN pip install sparrow
RUN pip install cartopy
RUN pip install torch_harmonics
RUN pip install modulus

RUN pip install hydra-core

HEALTHCHECK NONE
ENTRYPOINT [""]
