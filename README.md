How to run this example
------------------------

1. Clone this repository 

    git clone https://github.com/juancgalan/cmake-gtest-docker-example.git example

1. Change to the new directory
    
    cd example

1. Init submodules

    git submodule init

1. Update submodule (google test)

    git submodule update

1. Switch to build

    cd build

1. Generate make files

    cmake ..

1. Compile project

    make

1. Run tests

    make test


Runnig with Docker
------------------

1. Clone this repository 

    git clone https://github.com/juancgalan/cmake-gtest-docker-example.git example

1. Change to the new directory
    
    cd example

1. Init submodules

    git submodule init

1. Update submodule (google test)

    git submodule update

1. Run the docker compose command

    docker-compose run dev bash

1. Switch to the project directory

    cd /usr/src/app

1. Switch to build

    cd build

1. Generate make files

    cmake ..

1. Compile project

    make

1. Run tests

    make test


