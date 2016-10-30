# Schema Information

# Schema Information

## users
column              | data type |	 details
--------------------|-----------|---------------------------
id	                |  integer	| not null, primary key
email   	          |  string	  | not null, indexed, unique
username	          |  string	  | not null
password_digest     |	 string	  | not null
session_token	      |  string	  | not null, indexed, unique
admin               |  boolean  | default: false

## movies
column              | data type |	 details
--------------------|-----------|---------------------------
id	                | integer	  | not null, primary key
title	              | string	  | not null, indexed
description         | text      | not null
year	              | integer	  | not null
image_name          | string    |
image_type          | string    |
image_size          | integer   |
avg_rating	        | integer	  | default: 0


## genres
column          | data type |	 details
----------------|-----------|---------------------------
id	            | integer	  | not null, primary key
name            | string    | not null, indexed


## favorites
column          | data type |	 details
----------------|-----------|---------------------------
id	            | integer	  | not null, primary key
user_id         | integer   | not null, foreign key (references users), indexed


## reviews
column          | data type |	 details
----------------|-----------|---------------------------
id	            | integer   |	not null, primary key
user_id         | integer   | not null, indexed
rating          | integer   | not null, default: 0, indexed
body            | text      | not null

## castings (bonus)
column          | data type |	 details
----------------|-----------|---------------------------
id	            | integer   |	not null, primary key
series_id       | integer   | not null, indexed, foreign_key(references castings series table)
cast_id         | integer   | not null, indexed, foreign_key(references castings users table)

## actors (bonus)
column          | data type |	 details
----------------|-----------|---------------------------
id	            | integer   |	not null, primary key
name            | string    | not null, indexed
castings_id     | integer   | indexed, foreign_key(references castings join table)
