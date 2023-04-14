**Important: This work pre-dates [binaries and packages provided by Gazebo](https://gazebosim.org/docs/all/getstarted). To quick start, perhaps better to get those. Here is from source, with all it entails, like longer coffee breaks.**

# Ignite

Scripts to install and run Gazebo Ignition (current stable) from source.

Tested and working on U22. Supposed to support MacOS 12, but rought edges still (not tried on any other version).

## Install

### Requirements

* A recent Bash shell (no Bash magic in here, so recent means like the past 10 years should do).
* A Python 3 interpreter available.
* Optionally yet preferrably a Python virtual environment, as the install script gets some packages.

### The Install

From the root of the reposiotry:

    ./bin/prepare

 The script will require root access to install the Gazebo package repository key and install some dependencies (here using `apt`). No need to run with `sudo` or as privileged user; the script asks when it needs permission.
 
 A successful install does take some time, and ends with a success message explaining to use other scripts to run.
 
 ## Usage
 
 Two scripts are available, each run in its own shell:
 
     ./bin/server

Runs the simulation engine itself in headless mode. It is enough to many workflows.

    ./bin/gui

Runs the GUI client to the server, and requires an X11-ready environment.
