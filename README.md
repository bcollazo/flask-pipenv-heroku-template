# flask-pipenv-heroku-template

Minimal template for a heroku-ready Python 3 pipenv-enabled Flask app.

The purpose is to quickly start simple Flask apps ready for heroku, without
the repetive copy-pasting through the Flask Getting Started or the bloat of
the Heroku's https://github.com/heroku/python-getting-started tutorial.

## Using

Just clone into a new directory that you choose the name. Remove this .git
stuff associated with this repo, start a new .git, create heroku app, and push.

```
$ git clone https://github.com/bcollazo/flask-pipenv-heroku-template myappname
$ cd myappname
$ rm -rf .git
$ git init .
$ heroku create myappnameinheroku
$ git push heroku master
```

Now you can develop quickly by using:

```
FLASK_ENV=development FLASK_APP=app.py flask run
```

Edit your index.html, index.css, index.js appropriately, commit, and push! :)

## More info

This template was created by (and the repetitive tasks you skip are):

1. `pipenv install --three`
2. `pipenv install Flask`
3. Copy pasting hello.py from Flask's Getting Started
4. Adding Procfile with Gunicorn setup
5. Following Flask's Getting Started to add a index.html template connected
   to a index.css and index.js CSS and JS files.
