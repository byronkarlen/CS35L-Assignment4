# CS35L-Assignment4

### Assignment Spec
This assignment uses the development repository for the Time Zone Database (tzdb): 
https://github.com/eggert/tz
https://www.iana.org/time-zones 

Write a shell or Python script justone that displays the difference from the previous and current commit, assuming the repository is what an ordinary Git command would use.

Write a shell or Python script compare-releases that displays the difference between two tzdb releases given as arguments to the command. For example, compare-releases 2022f 2022g should output the difference between tzdb release 2022f and tzdb release 2022g.

Suppose we’re interested in the number of commits from each time zone. Write a shell or Python script tzcount that postprocesses the output of git log and outputs a simple report of time zones and number of commits from that time zone. Each line of output should look something like “-0500 1802”, meaning there were 1802 commits from the −0500 time zone. Use the commit date, not the author date, to determine the time zone of the commit. Sort the output numerically by its first (numeric timezone) column. Run the command git log 2012j..2022g | ./tzcount using the tzdb repository.

More info on the spec can be found here: 
https://web.cs.ucla.edu/classes/winter23/cs35L/assign/assign4.html
