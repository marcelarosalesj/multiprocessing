## Landing Algorithm

Problem:  
Suppose we have the elevation map of a region and we want an object (let's say a drone) to land somewhere there.  

This Algorithm checks the elevation map and selects "the best" place to land according to the differences in elevations of near pixels.


Compile for debugging:  
$ g++ -o sls sls.cpp `pkg-config opencv --cflags --libs` -lpthread -std=c++11 -g -v -da -Q

Run:  
./sls original 4 0.1
./sls <file in maps> <size> <difference>  

size is in pixels and 1px=10cm  
difference is in meters  
