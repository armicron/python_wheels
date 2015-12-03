apt-get install gcc g++ python-dev
pip install wheel

wget https://pypi.python.org/packages/source/p/pandas/pandas-0.17.1.tar.gz
tar xzvf pandas-0.17.1.tar.gz
cd pandas-0.17.1/
python setup.py sdist bdist_wheel


# How to install wheel
pip install wheel
pip install wheel_file.whl

or
pip install wheel
wget http://domain.com/wheel.whl
pip install wheel.whl