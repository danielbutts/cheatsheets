### [BACK](readme.md)

# Deploying Apps to Heroku with Postgres and Knex:

#### If Heroku CLI not already installed

1. Download and install CLI [Heroku Getting Started Guide](https://devcenter.heroku.com/articles/getting-started-with-nodejs#set-up)

2. Log into Heroku account

#### (otherwise)

1. commit latest code
- git add -A, git commit, etc.

2. heroku create <app-name>

3. git push heroku master

4. provision the heroku Postgres add-on
- heroku addons:create heroku-postgresql:hobby-dev

5. run migrations
- heroku run knex migrate:latest

5. run seeds
- heroku run knex seeds:run

7. heroku open
