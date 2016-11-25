###################################################################
# Dockerfile
#
# Version:          1
# Software:         BamM
# Software Version: 1.7.3
# Website:          https://github.com/Ecogenomic/BamM
# Provides:         BamM 1.7.3
# Base Image:       Alpine:3.3
# Build Cmd:        sudo docker build -t bamm_1.7.3-docker_img .
# Pull Cmd:         docker pull ecogenomics/bamm
# Run Cmd:          run -v `pwd`:/data bamm_1.7.3-docker_img parse
###################################################################
# Base image as Unbuntu
FROM alpine:3.3
# Copy in resources
COPY resources /tmp/ 
RUN ls /tmp/
RUN mv /tmp/bamm_1.7.3.tar.gz /
######################### Set up environment ######################
RUN tar xzf bamm_1.7.3.tar.gz
WORKDIR bamm_1.7.3
ENTRYPOINT ["/gnu/store/cp8dzw1mz95pddc7bdgad144dy94m9rs-profile/bin/bamm"]
