# SimpleApp
Django 3.2.1 LTS repo

https://www.youtube.com/channel/UCTZRcDjjkVajGL6wd76UnGg helpful resource

## Setup

### Create virtual environment

```bash
python -m venv env
source env/bin/activate
pip install -r requirements.txt
```
On Amazon Linux 2, I had to initially upgrade sqlite3

```bash
wget https://www.sqlite.org/2021/sqlite-autoconf-3350500.tar.gz
tar -xzf sqlite-autoconf-3350500.tar.gz
cd sqlite-autoconf-3350500
./configure && make && make install
mv /usr/bin/sqlite3 /usr/bin/sqlite3.bak
mv sqlite3 /usr/bin/sqlite3
cp /usr/bin/sqlite3 /usr/local/bin
export LD_LIBRARY_PATH="/usr/local/lib"
```
