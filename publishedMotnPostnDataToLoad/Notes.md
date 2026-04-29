Tim re-did the analyses after I spotted some errors and the [OSF site](https://osf.io/s4aqg/overview) has been updated.

Currently (19 Mar 2026), the raw data is not online. Instead, the most raw format is the MAT files, which calculates for each person for each of their two sessions the magnitude of their illusion. Tim says there remains a few discrepancies between the original MAT files and the CSV on OSF which is a couple participants that unexplainedly don't show up in the CSV.


Exclusion of participants was done at the illusion level (animations [here](https://tcottier96.github.io). There's different criteria listed in the paper for each illusion, which are correct. For the factor analysis, done in JASP, it was done both ways, any participant missing any illusion was completely excluded (list-wise exclusion) or just excluded for the relevant pairs (pair-wise exclusion).

Each illusion has at least 4 staircases, you run participant for fixed time, e.g. 160 trials, average over the last X trials for each staircase.  Never fit psychometric function for those illusions where staircases were used, just use 

Flash-grab effect, MIPS, and FJ do not have staircases, because they're using mouse or keyboard to adjust the stimulus.

MIPS: dva  (in the .MAT file)
FGE: arc-length distance in dva (in the .MAT file)
FJ: dva  likely (in the .MAT file) , Psychopy stuttered some so somewhat dodgy for temporal imprecision. 

waitBlanking was off for all the sessions and didn't check for whether any frames were too short

RT is also in the raw data.

Frohlich is always judgment relative to vertical (staircase sets the starting orientation on each trial). In flash-lag the bar flashes at a random orientation rather than always being at vertical.
