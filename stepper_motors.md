To start the motor controller:

open a terminal and switch user to nptest:
>su nptest
>
run the EPCS ioc as nptest
>cd $EPICS/app/iocBoot/iocThorLabs
>
>./st.cmd

open another terminal as nptest and run the motor controller which commnuicates with EPICS.
>cd v1
>
>./thor_epics -e

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

e.g.
>caput THOR_X:move_abs 69

open terminal run CSS
>/home/nptest/CSS/basic-epics-4.5.0/css
Say OK to default workspace.
