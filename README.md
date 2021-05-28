# Minimum Chat with Django Channels
This is a simple example how to create a non-styled chat with Websockets

#Getting Started

------------
##1- Install pipenv
```
pip3 install pipenv
pipenv shell
set PIPENV_VENV_IN_PROJECT=1
pipenv
```

##2- Install `docker` engine
Linux Instructions
------------
You can find instructions on the fabulous [docker documentation](https://docs.docker.com/engine/install/). Its important that you look for your distribution, for example, [for Ubuntu](https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository).

If you can install from repository or package manager, you should definitely do it.

Windows or Mac Instructions
------------

Once again docker's documentation for [Windows](https://docs.docker.com/docker-for-windows/install/) or [Mac](https://docs.docker.com/docker-for-mac/install/) is the place to go.

##3- Pull and run in the background a Redis service:
```docker run -p 6379:6379 -d redis:```

##4- Run the development server:

```python manage.py runserver 0.0.0.0:8000```

##5- Open your browser to [http:your-local-ip-here:8000/room/](http:your-local-ip-here:8000/room/)
Try using different devices accessing the same url and how the messages get updated in both.

Enyoy!!