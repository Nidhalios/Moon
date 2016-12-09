---
layout: post
project: true
title: "TV shows social plateform | NoSQL Project"
date: 2014-03-31
excerpt: ""
tags: [Spring MVC, Apache Cassandra, NoSQL, JAVA, J2EE, CQL]
comments: false
---

Since I was huge fan of TV shows and I wanted to get familiar with NoSQL databases, I got the idea to leverage my skills in J2EE and [Spring MVC](https://projects.spring.io/spring-framework/) Framework specifically to build a web application for TV shows' fans that writes and reads data from a column-oriented NoSQL database. I chose [Apache Cassandra](http://cassandra.apache.org) since it's one of most used NoSQL databases thanks to its fault-tolerance, linear scalability and high availability. it outperforms in fact most of the popular NoSQL alternatives. I used EasyCassandra ORM to interface between Cassandra and Spring Controllers. The following CQL script gives an idea on the database schema.

~~~~
CREATE KEYSPACE tvsnetwork WITH REPLICATION = { 'class' : 'SimpleStrategy', 'replication_factor' : 1};

CREATE TABLE Users (user_id uuid PRIMARY KEY, login text, pass text, first_name  text, last_name text, email text, dateOfBirth text, joinDate text, country text, points int);

CREATE TABLE TvShows (show_id int PRIMARY KEY, title text, launchDate text, directorName text, description text, network text, genres set<text>, image text); 

CREATE TABLE Actors (actor_id int PRIMARY KEY, first_name  text, last_name text, gendre text, dateOfBirth text, biography text, country text, image text);

CREATE TABLE User_TvShow (show_id int, user_id uuid, state text, PRIMARY KEY(show_id, user_id));

CREATE TABLE User_Actor (actor_id int, user_id uuid, PRIMARY KEY(actor_id, user_id));

CREATE TABLE Actor_TvShow (show_id int, actor_id int, role text, PRIMARY KEY(show_id, actor_id));

CREATE TABLE TvShow_Genre (show_id int, genre text, PRIMARY KEY(show_id, genre));
~~~~ 

<i class="fa fa-key" aria-hidden="true"></i>&nbsp;*Key Words:* Spring MVC, Apache Cassandra, NoSQL, JAVA, J2EE, CQL, NetBeans, EasyCassandra<br/>

*Application Screenshots*<br/>

![Home View](http://i.imgur.com/teBFwnE.png?1 "Home View")

![All Shows View](http://i.imgur.com/9fGProL.png?1 "All Shows View") 

![All Actors View](http://i.imgur.com/zGLFlwE.png?1 "All Actors View") 

![Actor Details](http://i.imgur.com/cjswNBa.png?1 "Actor Details") 

![Show Details](http://i.imgur.com/Nc28u7C.png?1 "Show Details") 








