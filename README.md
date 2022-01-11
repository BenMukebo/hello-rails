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

## Create Reals project

```bash
$   rails new hello-rails --database=postgresql  #use PostgreSQL database
$   cd hello-rails 
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


## Install gen pg

```bash
$   gem install pg  
```

## Run rails  

```bash
$   rails s    
```

## Generate Controller

- We need a Controller. Since everything goes through that, let's go ahead and generate one:

```bash
$  rails generate controller Pages hello 
```
- This should give us a Controller and a View

### Auto-correct

In auto-correct mode, RuboCop will try to automatically fix offenses:

```bash
$ rubocop -A
# or
$ rubocop --auto-correct-all
```
## Install unit tests

