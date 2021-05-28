# Deploy Keras Model with Flask as Web App 

A pretty and customizable web app to deploy your DL model with ease

## Getting Started

- Clone this repo 
- Install requirements
- Run the script
- Go to http://localhost:5000
- Done!

:point_down: Screenshot:

<p align="center">
  <img src="https://user-images.githubusercontent.com/5097752/71063354-8caa1d00-213a-11ea-86eb-879238887c1f.png" height="420px" alt="">
</p>


<p float="left">
  <img src="https://user-images.githubusercontent.com/5097752/71065048-61c1c800-213e-11ea-92f1-274cbe4734ba.png" height="330px" alt="">
  <img src="https://user-images.githubusercontent.com/5097752/71062921-aeef6b00-2139-11ea-8b23-6b9eb1e326ca.png" height="330px" alt="">
</p>

------------------

## Run with Docker

With **[Docker](https://www.docker.com)**, you can quickly build and run the entire application in minutes :whale:

```shell
# 1. First, clone the repo
$ git clone https://github.com/mtobeiyf/keras-flask-deploy-webapp.git
$ cd keras-flask-deploy-webapp

# 2. Build Docker image
$ docker build -t keras_flask_app .

# 3. Run!
$ docker run -it --rm -p 5000:5000 keras_flask_app
```

Open http://localhost:5000 and wait till the webpage is loaded.

## Local Installation

It's easy to install and run it on your computer.

```shell
# 1. First, clone the repo
$ git clone https://github.com/mtobeiyf/keras-flask-deploy-webapp.git
$ cd keras-flask-deploy-webapp

# 2. Install Python packages
$ pip install -r requirements.txt

# 3. Run!
$ python app.py
```

Open http://localhost:5000 and have fun. :smiley:

<p align="center">
  <img src="https://user-images.githubusercontent.com/5097752/71064959-3c34be80-213e-11ea-8e13-91800ca2d345.gif" height="480px" alt="">
</p>

------------------

## Customization

It's also easy to customize and include your models in this app.

<details>
 <summary>Details</summary>

### Use your own model

Place your trained `.h5` file saved by `model.save()` under models directory.

Check the commented code in app.py.

</details>

### Run the app

Run the script
```
$ python app.py
```

You can also use gunicorn instead of gevent
```
$ gunicorn -b 127.0.0.1:5000 app:app
```
