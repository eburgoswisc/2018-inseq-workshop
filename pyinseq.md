# Install Pyinseq

## Install Python on the remote instance

```
cd Downloads/
wget https://repo.continuum.io/archive/Anaconda3-4.4.0-Linux-x86_64.sh
chmod +x Anaconda3-4.4.0-Linux-x86_64.sh
./Anaconda3-4.4.0-Linux-x86_64.sh
```
Say "yes" to everything

```
cd ..
source ~/.bashrc
python
```

Should now see:

```
Python 3.6.1 |Anaconda 4.4.0 (64-bit)| (default, May 11 2017, 13:09:58)
[GCC 4.4.7 20120313 (Red Hat 4.4.7-1)] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

Type `exit()` to return to the bash shell.

## Install Pyinseq

```
pip install pyinseq
```
