# CPP Microservice

Study for building microservices in CPP using Conan and Poco.

## Installation

**Requirements**: Python 3.6+, pip, and a C++ compiler.  Built with clang 14.0.3 on OSX 13.4.1.  Recommend using a virtual environment in Python.  Built with a Conda environment.

1. `conda create -n cppms python=3.8`
2. `conda activate cppms`
3. `pip install conan`
4. `conan profile detect --force`
5. `conan install . --output-folder=build --build=missing`
6. `cmake .. -DCMAKE_TOOLCHAIN_FILE=conan_toolchain.cmake -DCMAKE_BUILD_TYPE=Release`
7. `cmake --build . --config Release`

More detail from ["Build a simple CMake Project using Conan"](https://docs.conan.io/2/tutorial/consuming_packages/build_simple_cmake_project.html).