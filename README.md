# odrSpiral
Exemplary implementation of Euler spirals as used for clothoids in OpenDRIVE. Originaly published by [VIRES Simulationstechnologie GmbH](https://vires.com/) in the publicly available [OpenDRIVE download section](http://opendrive.org/download.html).

## Building
### Building on Unix
With CMake as plattform-independent build tool **odrSpiral** can be configured for various native build environments. An exemplary configuration for Make under Unix:
```
cd odrSpiral
mkdir build
cd build
cmake ..
```
To build the project afterwards run
```
make
```
If everything went fine you will find the resulting library in the `lib/` folder of the project root.