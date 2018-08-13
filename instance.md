# Jetstream Remote Instance and Web Shell

## What is a remote instance?

You'll be renting a computer from Jetstream/XSEDE, an academic version of Cloud Computing (think, Amazon Web Services [AWS]). We have an "allocation" of compute resources from Jetstream for this workshop.

Most of the time, your instance will run Linux. Here we'll use the Ubuntu Linux operating system.

## Pros and cons of using a remote instance

Pros (big):
- Reproducible science: When you spin up a new instance and do the analysis from scratch, you know exactly how to reproduce that analysis.
- Increased compute capacity.
- Can run different operating systems (e.g. Run a unix system from a Mac or PC).
- Does not tie up your computer.

Cons (small):
- Need to connect to the instance:
    - Web shell: Easy to get started.
    - SSH: Use for web-independent connection, moving files to your local machine.
- Will not work unless you provide everything for the analysis.
- Typically you are working with a Linux server, so all functions are through the command line.


## Set up your instance

[Follow these instructions from the DIB Lab](https://2017-dibsi-metagenomics.readthedocs.io/en/latest/jetstream/boot.html) with the following changes:
- Use this image: `s1.large (CPU: 10, Mem: 30 GB, Disk: 120 GB, Disk: 120 GB root)`, but an `m1.medium` instance will likely work too.

## Open the web shell

Click on the instance and, once it is running, open the "Web Shell". This provides a web interface to the instance's command line.