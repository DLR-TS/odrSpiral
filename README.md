# odrSpiral
Exemplary implementation of Euler spirals as used for clothoids in OpenDRIVE. Originaly published by [VIRES Simulationstechnologie GmbH](https://vires.com/) in the publicly available [OpenDRIVE download section](http://opendrive.org/download.html):

> This small collection of routines shall illustrate the computation of Euler spirals as they are to be used in OpenDRIVE applications.
>  
> The methods have been realized using the CEPHES library 
> 
> http://www.netlib.org/cephes/
>
> and do neither constitute the only nor the exclusive way of implementing spirals for OpenDRIVE applications. Their sole purpose is to facilitate the interpretation of OpenDRIVE spiral data.
>
> All software is provided "AS IS".

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
If everything went fine you will find 
- the resulting static library in the `lib/` folder of the project root and 
- an `odrSpiralDemo` executable in the `bin/` folder.
  > Running it will result in a table of x/y values for a sample spiral.