# ccs8803-env_Jutul
Docker environment for JutulDarcy simulation for CCS8803 class

This repository contains a dockerfile and julia notebooks for running numerical
experiments around carbon capture sequestration (CCS) in a prebuild environment.

To build the image do

`> docker build -t ccsenv:1.0 --platform linux/x86_64 .`

To run the image run

`> docker run --platform linux/x86_64 -p 8888:8888 -v "${PWD}":/notebooks ccsenv:1.0`

from within the parent directory of notebooks.

