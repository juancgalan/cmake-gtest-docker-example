How to run this example
------------------------

1. Clone this repository 

```sh
git clone https://github.com/juancgalan/cmake-gtest-docker-example.git example
```

1. Change to the new directory
```sh
cd example
```
1. Init submodules
```sh
git submodule init
```
1. Update submodule (google test)
```sh
git submodule update
```
1. Switch to build
```sh
cd build
```
1. Generate make files
```sh
cmake ..
```
1. Compile project
```sh
make
```
1. Run tests
```sh
make test
```

Runnig with Docker
------------------

1. Clone this repository 

```sh
git clone https://github.com/juancgalan/cmake-gtest-docker-example.git example
```

1. Change to the new directory
```sh
cd example
```
1. Init submodules
```sh
git submodule init
```
1. Update submodule (google test)
```sh
git submodule update
```
1. Run the docker compose command
```sh
docker-compose run dev bash
```
1. Switch to the project directory
```sh
cd /usr/src/app
```
1. Switch to build
```sh
cd build
```
1. Generate make files
```sh
cmake ..
```
1. Compile project
```sh
make
```
1. Run tests
```sh
make test
```
