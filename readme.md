# Scalable Deep Learning Model Prediction Server with Redis
This was built following [this tutorial](https://pyimagesearch.com/2018/02/05/deep-learning-production-keras-redis-flask-apache/)
## Usage / Development
Install dependencies with:
```
$ pip install -r requirements.txt
```
Then, use [`launch-redis.sh`](/launch-redis.sh) to spin up a local redis instance using Docker.
Then, run:
```
$ python run_model_server.py
```
and
```
$ python run_web_server.py
```
to start the model and web servers.
Finally, run:
```
$ python simple_request.py
```
to execute a single request, or:
```
$ python stress_test.py
```
to execute 50 concurrent requests.