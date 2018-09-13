# mcl_ws

=====

**Dependencies**
*DON"T DO THIS IF YOU ARE ON VLabs!!!*

```
sudo apt-get install libcv-dev
sudo apt-get install libcvaux-dev libhighgui-dev
sudo apt-get install python-numpy python-opengl
sudo apt-get install swig
```


**Build & Run**
```
cd mcl_ws
rm -r devel build
catkin_make
source devel/setup.bash
cd src/no_weights/src/raycaster
make clean
make
cd ../../../with_weights/src/raycaster
make clean
make
```

Now run:
```
roslaunch uml_mcl mcl.launch
rosrun no_weights no_weights.py
#or
rosrun with_weights with_weights.py
```


