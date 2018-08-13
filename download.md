# Download results

## Web shell

We [discussed](instance.html) some of the methods to download results. Here we will download the results file from using the web shell.

`CTL-CMD-SHIFT` to open sidebar

Click on the icon in `Devices`

Click on the following folders:
- home
- mmandel (well, your name)
- results
- example2

Double-click on desired files to download. Focus on:
- log.txt
- samples.yml
- summary_gene_table.txt


## Alternate Method: Dropbox

Sign up for Dropbox account. Separate account than your main one. You will end up sharing a folder between the accounts.

Set up the shared folder. Make a folder in your main account, invite your new account. Log into your new account (web site) and accept the invitation ("Add to Dropbox")

[Install Dropbox on the server](https://www.dropbox.com/install-linux)

```
cd ~ && wget -O - "https://www.dropbox.com/download?plat=lnx.x86_64" | tar xzf -
```

Run Dropbox:

```
~/.dropbox-dist/dropboxd
```

Authenticate in a browser using the provided URL.

Download python script to control Dropbox:


```
cd

mkdir scripts

cd scripts

wget https://www.dropbox.com/download?dl=packages/dropbox.py
```

For easy access, put a symlink to the script anywhere in your PATH.
