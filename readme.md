# Python3

```
cd ~/packages
tar xf Python-3.5.4.tgz
cd Python-3.5.4/
mkdir /export/home/boshin/py354
./configure --prefix=/export/home/boshin/py354
make
make install
```


```
sh Anaconda2-4.2.0-Linux-x86_64.sh -b -p ~/conda
~/conda/pip 
```



# Virtualenv

* copy all package files to ~/packages

```
cd ~/packages
/export/home/boshin/py354/bin/pip3 install --no-index --user --find-links=./ virtualenv
/export/home/boshin/.local/bin/virtualenv -p /export/home/boshin/py354/bin/python3 ~/virt/k3
source ~/virt/k3/bin/activate
```


# Install requirements

```
~/packages
pip install numpy --no-index --find-links=./ 
pip install tensorflow-gpu --no-index --find-links=./ 
pip install keras --no-index --find-links=./ 
pip install spacy --no-index --find-links=./ 
pip install torchvision --no-index --find-links=./ 
pip install torchvision --no-deps --no-index --find-links=./ 
pip install boto3 --no-index --find-links=./ 
pip install webencodings --no-index --find-links=./ 
pip install progressbar33 --no-index --find-links=./ 
pip install ipdb --no-index --find-links=./ 
pip install lazy_property --no-index --find-links=./ 
pip install cython --no-index --find-links=./ 
pip install colorlog --no-index --find-links=./ 
pip install ./en_core_web_md-1.2.0.tar.gz
python -m spacy link en_core_web_sm en
```

boto3
webencodings-0.5.1
progressbar33
ipdb
lazy_property
cython0.22
colorlog==3.0.0
