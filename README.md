# hello-rails

## Learning objectives

- Install Ruby on Rails framework.
- Use RubyGems as a software package system.

## Setup

### Clone this repository

```bash
$ git clone https://github.com/BenMukebo/hello-rails.git
$ cd hello-rails
```


## Installing Rails

- To install Rails, use the `gem install` command provided by RubyGems:

```bash
$   gem install rails
$   gem install rails -v 5.2.0 
```

- To verify that you have everything installed correctly, you should be able to run the following in a new terminal:

```bash
$   rails --version
```

## Creating the hello-rails Application

- use PostgreSQL database 

```bash
$   rails new hello-rails --database=postgresql  #or
$   rails new hello-rails -d postgresql

$   cd hello-rails # Move into the application directory
```


### Create the database

```bash
$   rails db:create   # or
$   rake db:create
```

### Starting up the Web Server

```bash
$   rails s # or
$   rails server 
```


- You can now visit `http://localhost:3000` to view your new website!

```bash
$   http://localhost:3000/ # to see your changes in action.
```


<!-- ## Err

```bash
$  sudo dpkg --configure -a
$  sudo apt-get install ruby-dev build-essential   
``` -->

## Fix Error

```bash
$   sudo apt-get install libpq-dev  
```


#### Install gen pg

```bash
$   gem install pg  
```



#### Generate Controller

- We need a Controller. Since everything goes through that, let's go ahead and generate one:

```bash
$  rails generate controller Pages hello 
```
- This should give us a Controller and a View



#### Listing Existing Routes

- To get a complete list of the available routes in your application, visit

```bash
$  http://localhost:3000/rails/info/routes
```

 You can also execute the `rails routes` command in your terminal to produce the same output.

## Setting Up PostgreSQL

- Install a recent version of Postgres.

```bash
$   sudo apt install postgresql-11 libpq-dev
```

- The postgres installation doesn't setup a user for you, so you'll need to follow these steps to create a user with permission to create databases

<!--  sudo -u postgres createuser -s magnusben -P -->

```bash

$  sudo -u postgres createuser magnusben -s
# If you would like to set a password for the user, you can do the following
$ sudo -u postgres psql
$ postgres=
```

