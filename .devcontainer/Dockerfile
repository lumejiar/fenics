FROM ghcr.io/scientificcomputing/fenics-gmsh:2024-05-30

# Instalar herramientas adicionales
RUN apt-get update && apt-get install -y \
    git \
    vim \
    nano \
    wget \
    curl \
    && rm -rf /var/lib/apt/lists/*

# Instalar paquetes Python adicionales
RUN pip3 install --no-cache-dir \
    numpy \
    matplotlib \
    scipy \
    pandas \
    jupyterlab

# Configurar directorio de trabajo
WORKDIR /workspaces
