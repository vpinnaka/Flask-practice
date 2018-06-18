# Flask-practice
Repository to practice flask applications

### Deploying app to Heroku
* Login to heroku from command line (download Heroku CLI [here](https://devcenter.heroku.com/articles/getting-started-with-python#set-up))
```
$ heroku login
Enter your Heroku credentials.
Email: python@example.com
Password: *******
```
* Use the boiler-plate code from [this](.) repository and clone it to your local
```
$ git clone https://github.com/vpinnaka/Flask-practice/tree/1.0
$ cd Flask-practice
```
* Install all the requirements (Use `pipenv` for convineance)
```
$ pip install pipenv
$ pipenv install
$ pipenv install -r requirements.txt
```
* Create a file named `Procfile` with following content (If it does not exist)
```
web: gunicorn app:app
```
* Create  a app in Heroku
```
$ heroku create your-app-name
```
* Push your code to Heroku master
```
$ git push heroku master
```