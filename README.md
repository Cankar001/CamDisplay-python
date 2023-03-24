# CamDisplay

The CamDisplay is another client for the CamServer, 
but instead of reading and analyzing the video feed, 
it will receive all current frames from the server 
and simply display them onto the screen.

The use case could be a raspberry with an attached 
raspberry screen, which can be placed anywhere 
in the house and where everyone could see the live 
feed of the camera all the time.

# Getting started

## Clone the repository
```shell
git clone https://github.com/Cankar001/CamDisplay.git
```

## Create a environment file
You need to copy the `.env.example` file and rename it to just `.env`.

Fill in the server address and the port, you chose before when intializing the server.

## Create a virtual environment
```shell
python -m venv venv
```

## Activate the virtual enviroment
```shell
# on windows
.\venv\Scripts\activate.bat

# on linux
source ./venv/bin/activate
```

## Check if environment has been activated
```shell
# This command should show the python path,
# pointing to your venv folder
pip --version
```

## Install requirements from requirements.txt
```shell
pip install -r requirements.txt
```

## Run client
```shell
pipenv run python Client.py
```

# Troubleshooting

I discovered, that the virtualenv doesn't seem to like the powershell, 
I couldn't get it working in it.

But using a bash on windows, using `source ./venv/Scripts/activate` worked perfectly fine.
