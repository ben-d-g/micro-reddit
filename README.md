# micro-reddit

From [The Odin Project](https://www.theodinproject.com/lessons/ruby-on-rails-micro-reddit)

Let’s build Reddit. Well, maybe a very junior version of it called micro-reddit. In this project, you’ll build the data structures necessary to support link submissions and commenting. We won’t build a front end for it because we don’t need to… you can use the Rails console to play around with models without the overhead of making HTTP requests and involving controllers or views.

## schema

User:

- username - string[5,15], primary key, alphanumeric

Post:

- post_id - integer, primary key
- username - foreign key, not null
- title - string, not null
- content - text

Comment:

- post_id - foreign key
- username - foreign key
- content - text