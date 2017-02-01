slurm-scripts
=============

This is a collection of some very simple one-line shell scripts for
managing your SLURM jobs on a HPC cluster.  Take what appears
useful to you and adapt it to your needs.  If you feel like it, add
your own contributions (pull requests welcome).

To use these, download the scripts and put them into a directory in
your `$PATH` like `~/bin/`, e.g.:

```
cheops0:~$ git clone http://github.com/maxhgerlach/slurm-scripts
cheops0:~$ mkdir ~/bin
cheops0:~$ cd ~/bin
cheops0:~/bin$ ln -s ~/slurm-scripts/* -t .
```

The folder `old-torque-scripts` contains some scripts that were
written for older installations with the Torque/Maui scheduler.  These
will not work on more recent systems, but since SLURM provides a lot
of their functionality on its own, most of them are not really needed
any more anyway.
