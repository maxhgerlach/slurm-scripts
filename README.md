cheops-scripts
==============

While Torque provides quite a few commands to manage jobs on the
Cheops cluster, some operations are unnecessarily tedious.  This is a
collection of some rather simple shell and python scripts that could
make things slightly more enjoyable.  Take what
appears useful to you and adapt it to your needs.  If you feel like it,
add your own contributions.

To use these, download the scripts and put them into a directory in
your `$PATH` like `~/bin/`.

### qstatme

`qstat`, but only list your own jobs

### qstatnames

Pure `qstat` always truncates the names of your jobs to 12 characters,
which may not be enought to tell them apart precisely.  This script
prints the ids and full names of all your jobs.  Since for each job a
separate call to `qstat` is made, this can be slow if you have a lot
of jobs in the queue.  Improvements are welcome.

### qtwins

Prints the ids of all your jobs that have matching full names.

### qgrep

Grep from the names of your jobs and return a list of matching job
ids. `qgrep -E REGEX` also works.

### qgrepdel

Grep from the names of your jobs and delete all matching jobs.
`qdelgrep -E REGEX` also works.

### qpeekout, qpeekerr

These print what has been written so far to the standard output or
error stream of a job *while it is still running*.  With these scripts
there is no need to specify any redirections in the job scripts.

### qlast

Print the jobid of the last job you have submitted.  This is useful
for tasks like `qpeekout $(qlast)`.

### qstatlast

Print full job information for the last job you have submitted.

### hereon, hereoncheops

`hereon` simply connects to some other host (like a cluster node) and
puts you into the current directory from the start.  `hereoncheops` is
useful to do the same when you want to switch from your workstation to
the cluster.  Make sure to put in your own user names.

### countmynodes, countmycores

just vanity
