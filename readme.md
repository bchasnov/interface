Dynamics of human/machine interactions.

## Instructions

### Installation
Create a virtual environment `env` and install required packages.
```
virtualenv -p python3 env
env/bin/activate
pip install -r requirements.txt
```

### Run the browser app
Host the website locally
```
livereload web/index.html
```
and go to `http://localhost:35729/`.

### Run the websocket daemon
Connect a physical device to the web interface
```
python scripts/webinput.py --device "COM4" --port 4567 
```

## Functionality
Supported tasks:
* Continuous reference tracking

Supported systems:
* First- and second-order systems

Supported physical devices:
* Mouse+keyboard (via the browser)
* Serial port (via a websocket daemon)

