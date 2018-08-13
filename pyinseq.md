# Install Pyinseq

## Install Python on the remote instance

```
cd Downloads/
wget https://repo.continuum.io/archive/Anaconda3-5.2.0-Linux-x86_64.sh
chmod +x Anaconda3-5.2.0-Linux-x86_64.sh
./Anaconda3-4.4.0-Linux-x86_64.sh
```
`yes` to license
Default install location (hit `enter`)
`yes` to prepend in path
`no` to install VSCode

```
cd ..
source ~/.bashrc
python
```

Should now see:

```
Python 3.6.5 |Anaconda, Inc.| (default, Apr 29 2018, 16:14:56)
[GCC 7.2.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```

This is the python shell (also called the REPL).
You can now run python on your remote instance, and the command `python` points to the version to just installed.
Type `exit()` to return to the bash shell, which will look something like this:

```
mmandel@js-170-233:~$
```


## Install Pyinseq

Install the latest version from GitHub:

```
pip install --upgrade pip
pip install git+git://github.com/mandel01/pyinseq
```

If you want to install the version registered in the Python Package Index, instead type `pip install pyinseq`.


## Upload data to the instance

Make and enter the data directory

```
mkdir data
cd data
```

Download the sample data

```
wget https://www.dropbox.com/s/icroinqkyev4bb3/pyinseq_example_files.tar.gz
tar -zxvf pyinseq_example_files.tar.gz
```

## Run pyinseq

Check out the required arguments:

```
pyinseq
```


Run a tiny dataset:

```
cd
pyinseq -i data/example01.fastq -s data/example01.txt -g data/ES114v2.gb -e example1

```


Run a larger dataset:

```
cd
pyinseq -i data/example02.fastq.gz -s data/example02.txt -g data/ES114v2.gb -e example2

```