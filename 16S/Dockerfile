FROM condaforge/mambaforge

LABEL base.image="ubuntu:mambaforge"
LABEL dockerfile.version="1"
LABEL software="barrnap"
LABEL software.version="0.9"
LABEL description="Barrnap with bedtools and biopython included"
LABEL pipeline="Juno-typing"
LABEL conda_file_hash="REPLACE_HASH"

# RUN apt-get update && apt-get install -y --no-install-recommends \
#   tree

# RUN tree -L 3

COPY environment.yaml .
RUN /bin/bash -c "mamba env update -n base -f environment.yaml"