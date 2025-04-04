# README

This README would normally document whatever steps are necessary to get the
application up and running.

Install ruby 3.2.2

Install rails 7.2.2.1

Install postresql 

sudo service postgresql start
sudo -u postgres psql
CREATE ROLE postgres WITH SUPERUSER CREATEDB CREATEROLE LOGIN;
ALTER USER postgres WITH PASSWORD 'PASSWORD';
CREATE ROLE rails LOGIN PASSWORD 'rails';
ALTER ROLE rails CREATEDB;

Install Redis server
sudo apt install redis-server
redis-server

bundle install

rails db:setup
OR
rails db:create

rails db:migrate

open localhost:3000 in two browser tabs
