In order to setup the workspace:

```mkdir -p ~/catkin_ws/src && cd ~/catkin_ws/src```

```git clone https://github.com/alexperez33/car_example.git```


To provide nice alias for starting rviz with the indyav.rviz config (and for starting gazebo), run the script in the scripts directory.

```cd ~/catkin_ws && catkin_make```

It might fail due to the fact that it "can't find indyav_control". Just compile that package first:
```catkin_make indyav_control_gencpp```

Then redo the ```catkin_make```.

To demo the indycar, simply run:
```roslaunch indyav_launch gazebo.launch```

If you ran the script from earlier, you can simply run this command to open rviz:
```indyviz```

If you wish to see the car in gazebo:
```gazebogui```
