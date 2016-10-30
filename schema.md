# Schema Information

## users
column name     | data type | details
----------------|-----------|-----------------------
id              | integer   | not null, primary key
username        | string    | not null, indexed, unique
email           | string    | not null, indexed, unique
password_digest | string    | not null
session_token   | string    | not null, indexed, unique

## movies
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
title       | string    | not null
description | text      | not null


## actors
column name | data type | details
------------|-----------|-----------------------
id          | integer   | not null, primary key
movie_id    | integer   | not null, foreign key (references movies id), indexed
name        | string    | not null
