## Setting up sbs-offline and sbs replay
Follow Sebastian's guide


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
