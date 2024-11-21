## Setting up sbs-offline and sbs replay
Follow Sebastian's guide: 
https://sbs.jlab.org/DocDB/0004/000423/010/Hall_A_Analysis_Software_Installation_Guide%20v9.pdf

### Git updates
some Gitupdates to replay/offline might break the replaying.
If this happens you may need to rebuild SBS-offline (and maybe analyzer too).

To do this, simply remove the build and install contents in SBS-offline like so.
>cd $SBS/../build
>rm * -rf
>
>rm ../install/* -rf

You can then rebuild as per Sebastian's guide:
>cd build
>
>cmake -DCXXMAXERRORS=1 -DCMAKE_BUILD_TYPE=RelWithDebInfo -DCMAKE_INSTALL_PREFIX=../install -S ../SBS-offline/
>
>make install


## Replaying scripts
>sbsoffline/install/run_replay_here
>
>.L <replay_script>.C+
>
>replay_script(<run_number>)

## Raw .evio file locations
### stored files
raw files not used for some time will be sent to tape.
the locations for files before they are sent to tape is:
- adaqeb[1-3]/data/
- adaq1/data1/sbs/
- cache/mss/halla/sbs/raw/
- cache/mss/halla/sbs/GEnRP/raw
- cache/halla/sbs/GEnRP/raw

### tape files
If the files are not in the above storage locations they will need to be retrieved from tape.

tape storage is at
>/mss/halla/sbs/GEnRP/raw/
>
>jcache get /path/to/file.evio
