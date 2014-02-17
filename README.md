# Mesos Tutorial

## Install mesos

Follow [this instruction](http://mesos.apache.org/gettingstarted/).
If you are on OSX 10.9 (Maverick), you need to download gcc47 before compiling mesos. And compile mesos with gcc.
```
brew install gcc47
cd path/to/mesos
mkdir build
cd build
CC=gcc-4.7 CXX=g++-4.7 ../configure
```

## Run mesos locally

Run master:
```
./path/to/bin/mesos-master.sh
```

Run slave:
```
./path/to/bin/mesos-slave.sh --master=localhost:5050
```

## Run hadoop on mesos

Follow [this instruction](https://github.com/mesos/hadoop)
