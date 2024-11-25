## To start the motor controller:

open a terminal and switch user to nptest:
```bash
su nptest
```
run the EPCS ioc as nptest
```bash
$EPICS/app/iocBoot/iocThorLabs
./st.cmd
```

open another terminal as nptest and run the motor controller which commnuicates with EPICS.
```bash
cd ~/v1
./thor_epics -e
```

### Move it move it
you should now be able to run EPICS commands to read and move the motor.
The EPICS channels are:

Readback (preface this with caget): 
- THOR_Y:read_pos
- THOR_X:read_pos
- THOR_Y:read_stat
  
Command (preface this with caput):
- THOR_Y:move_abs
- THOR_X:move_abs
- THOR_Y:move_home

examples of commands:
```bash
caput THOR_X:move_abs 69
caget THOR_Y:read_pos
```

These commands can be put into shell scripts:

see examples of a this in 
>/home/nptest/v1/

## GUI

If you want a GUI you can use the following:
open terminal run CSS
>/home/nptest/CSS/basic-epics-4.5.0/css
Say OK to default workspace.
