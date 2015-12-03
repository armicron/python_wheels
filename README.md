System requirements
===================
Wheel's build is very system-specific.
For shippable/minv2 testing container we should use ubuntu 12.04 (or minv2 itself, but it's size is around 10Gb)
```
docker pull ubuntu:12.04
docker run -i -t ubuntu /bin/bash
```
Preparing environment
=========================================
```
apt-get install gcc g++ python-dev
virtualenv env
source env/bin/activate
```

How to build a wheel
==================

```
pip install wheel
wget https://pypi.python.org/packages/source/p/pandas/pandas-0.17.1.tar.gz
tar xzvf pandas-0.17.1.tar.gz
cd pandas-0.17.1/
python setup.py sdist bdist_wheel
```

How to install a wheel
====================

```
pip install wheel_file.whl
```

or

```
wget http://domain.com/wheel.whl
pip install wheel.whl
```
