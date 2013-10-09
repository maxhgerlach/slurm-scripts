cheops-scripts
==============

This is a collection of some very simple one-line shell scripts for
managing your SLURM jobs on the CHEOPS cluster.  Take what appears
useful to you and adapt it to your needs.  If you feel like it, add
your own contributions.

To use these, download the scripts and put them into a directory in
your `$PATH` like `~/bin/`, e.g.:

```
cheops0:~$ git clone http://github.com/maxhgerlach/cheops-scripts
cheops0:~$ mkdir ~/bin
cheops0:~$ cd ~/bin
cheops0:~/bin$ ln -s ~/cheops-scripts/* -t .
```

The folder `old-torque-scripts` contains some scripts
that were written for the previous installation with the Torque/Maui scheduler.  These
will not work any more, but since SLURM provides a lot of their
functionality on its own, most of them are not really needed any more
anyway.
