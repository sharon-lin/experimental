Notes
=====

You can try out our site: http://obscure-island-8606.herokuapp.com/

Username: dchacks
Password: expresso

Deploying to Heroku
-------------------

You can simply create your own copy on heroku with following steps:

Clone repository:

    $ git clone git@github.com:mrhead/notes.git

Create heroku app:

    $ cd notes
    $ heroku create [your_app_name]
    $ git push heroku master
    $ heroku run rake db:migrate # in case of connection issues run: heroku run:detached rake db:migrate

Set your login and password:

    $ heroku config:set login=your_login
    $ heroku config:set password=your_password

And open it in the browser:

    $ heroku open

Enjoy it!
