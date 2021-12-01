# Tensorflow Lite for mbed

Extraction of Tensorflow Lite as a library for use with mbed cli projects.

```sh
mbed add https://github.com/sillevl/tensorflow-lite-micro-mbed.git
```

## Hello World application

An example of the hello world application using this library can be found at: https://github.com/sillevl/tensorflow-lite-micro-hello-world-mbed

## Building the library

The library is build using a _helper_ docker container. The project is available at [sillevl/tensorflow-lite-micro-docker-mbed-helper](https://github.com/sillevl/tensorflow-lite-micro-docker-mbed-helper) at GitHub.

```sh
docker run -it --rm -v ${pwd}:/tensorflow/hello_world/ tf-lite-mbed python3 tensorflow/lite/micro/tools/project_generation/create_tflm_tree.py /tensorflow/hello_world/
```
