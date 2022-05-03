# Micro-Reddit
This repo contains the data models for how Reddit's User/Post/Comment system works. No front-end is currently implemented. 
The Reddit posting system works as follows:
> A User has_many Posts & has_many Comments

> A Post belongs_to a User & has_many Comments

> A Comment belongs_to a Post & belongs_to a User

There are three SQL tables, User, Post, and Comment. Post contains a reference column to user_id and Comment contains two reference columns for user_id and post_id. This data model enables multiple users to make and comment on posts and have their usernames displayed when they do so, like how Reddit operates.
