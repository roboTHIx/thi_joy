# roboTHIx joy for ROS 2

Package for implementing different gamepads to use it in the ROS 2 Galactic roboTHIx environment.


## Known Issues

  -


## Prerequisites for PS 4 Gamepad

  - [`naoki-mizuno/ds4drv`](https://github.com/naoki-mizuno/ds4drv/tree/devel) (`devel` branch)
    ```
    git clone https://github.com/chrippa/ds4drv.git
    cd ds4drv
    sudo python setup.py install
    ```
    
  - [`naoki-mizuno/ds4_driver`](https://github.com/naoki-mizuno/ds4_driver/tree/foxy-devel) (`foxy-devel` branch)
    ```
    mkdir -p ~/ws_ds4_driver/src
    cd ~/ws_ds4_driver/src
    git clone https://github.com/naoki-mizuno/ds4_driver.git --branch foxy-devel
    cd ~/ws_ds4_driver
    colcon build
    source install/setup.bash
    ```


## Getting Started

To pull packages, install dependencies, compile, and source the workspace
```
git clone https://github.com/roboTHIx/thi_joy.git ws_thi_joy/src
cd ~/ws_thi_joy
colcon build
source install/setup.bash
```


## Packages in the Repository

  - `thi_ps4` 
    - `ps4_cmd_vel` ps4 gamepad to cmd_vel output
    - `ps4_jogarm` controll a robotarm with the ps4 gamepad using moveit2
    - `ps4_joy` ps4 gamepads to joy output
    - `ps4_rviz` controll rviz view with the ps4 gamepads touchpad



## Usage



## Expected Changes in the Near Future

  - Create packages for more gamepads
  
