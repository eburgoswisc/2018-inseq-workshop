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
    - SSH: Use for web-independent connection.
- Cumbersome to move files back and forth.
- Typically you are working with a Linux server, so all functions are through the command line.


## Ways to move files in & out of the instance:

- Atmosphere Web Shell / Web Desktop. Not sure if this works for larger (GB) files.
- `wget` to import files from a URL (e.g., Dropbox, box.com, web site).
- Dropbox to download (sync) files: Limited to size of Dropbox account.
- SSH + SCP


## Note about SCP

If adding SSH keys for secure copy (SCP) to get files off the server at the end of the run – need to add the keys before launching the instance.

[Adding SSH keys to the Jetstream Atmosphere environment](https://iujetstream.atlassian.net/wiki/spaces/JWT/pages/17465474/Adding+SSH+keys+to+the+Jetstream+Atmosphere+environment)

[Logging in with SSH](https://iujetstream.atlassian.net/wiki/spaces/JWT/pages/17465502/Logging+in+with+SSH)


## Set up your instance

[Follow these instructions from the DIB Lab](https://2017-dibsi-metagenomics.readthedocs.io/en/latest/jetstream/boot.html) with the following changes:
- Use this image: `s1.large (CPU: 10, Mem: 30 GB, Disk: 120 GB, Disk: 120 GB root)`, but an `m1.medium` instance will likely work too.


## Managing and deleting your instance

Changes in the instance can take up to 15 minutes to fully take effect.

You must delete the instance to fully stop using resources.

“Your instance will be shut down and all data will be permanently lost!”

Can Suspend (think "Sleep" on your laptop) or Stop (think "Shutdown") an instance if you want to save the data temporarily and return to it, but have to remember to return to it and then to Delete.

If you want to shutdown your instance and return to it much later, consider "Shelve" as an option.

[More info on these instances and on troubleshooting deployment](https://iujetstream.atlassian.net/wiki/display/JWT/Instance+management+actions)


## Open the web shell

Click on the instance and, once it is running, open the ["Web Shell"](https://calvinmclean.github.io/atmosphere-guides/guacamole_user_guide.html). This provides a web interface to the instance's command line.


### Check out the sidebar

`CTL-ALT(CMD)-SHIFT` opens or closes the sidebar.

Copy & Paste:
- Paste from your computer: Paste your text into the text box. Close the sidebar. Right click to paste in the command line.
- Copy to your computer: Highlight text. Open the sidebar. Highlight and copy. Paste on your local machine.

File Transfer:
- Click on Devices. Click to desired location
    - Upload: Click "Upload File" and select file to upload.
    - Download: Double-click on the desired file.
