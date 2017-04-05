## Distributed Health App

## Setup

```
$ virtualenv flask
$ source flask/bin/activate
$ pip install -r requirements.txt
```

### Start Server

Start the Flask server in the virtual environment

```
$ ./run.py
```

### Interact with Server

In a new terminal window, run the following:

```
$ python3
>>> import requests
>>> response = requests.post('http://127.0.0.1:5000/update', data = {'user':'A', 'vector':'.1,.2,.3,.5'})
>>> response.json()
```
