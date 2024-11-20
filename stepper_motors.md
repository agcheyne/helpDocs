To start the motor controller:

open terminal and run the EPCS ioc
>cd $EPICS/app/iocBoot/iocThorLabs
>./st.cmd

open terminal run the motor controller which commnuicates with EPICS.
>cd v1
>./thor_epics -e

The EPICS channels are:
Readback: "THOR_Y:read_pos", "THOR_X:read_pos", "THOR_Y:read_stat","THOR_X:read>
Command: THOR_Y:move_abs,THOR_X:move_abs,THOR_Y:move_home,THOR_X:move_home, THO>

open terminal run CSS
>/home/nptest/CSS/basic-epics-4.5.0/css
Say OK to default workspace.
