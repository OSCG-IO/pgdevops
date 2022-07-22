# pgDevOps #

pgDevOps is a multi-user & multi-server PostgreSQL dev-ops web console that features integration with pgAdmin4.  

It's a WSGI Python Flask application that runs cross-platform (Windows, OSX & Linux) in Crossbar. pgDevOps is AGPLv3 licensed Open Source software.


### Setup python3 env

```
#!bash
python3 -m venv devops-env
source tutorial-env/bin/activate
git clone https://github.com/oscg-io/pgdevops
cd pgdevops
pip3 install -r requirements.txt

```

### Setup admin user (shared by pgDevOps and pgAdmin4 Web)
```
#!bash

python3 pgadmin/setup.py

```

### Startup crossbar
```
#!bash

export MY_HOME="$HOME/c/oscg"
export MY_LOGS="$MY_HOME/logs/pgcli_log.out"
./bin/start_crossbar.sh

```
