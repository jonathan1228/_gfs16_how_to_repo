# Git CheatSheet

### Start a new project

```shell
$ mkdir project_name
$ git init
$ touch readme.md
$ git add readme.md
$	git commit -m "initial commit"
```

### Do some work and then save it

First, do some work!

```shell
$ git status
$ git add <whatever file>
$ git status
$ git commit -m "I made a bunch of changes, there are so many details, wee."
```

### Share my work with the world!

First, create a github repo.

```shell
$ git remote add origin git@github.com:<github username>/<name of repository>.git
$ git push -u origin master
```

### Help someone else with their code

First, find the code on githb that you want to contribute to.
Then Fork it!

```shell
$ git clone git@github.com:<your username>/_How_to_Repo.git
```

Then, make some changes you think are important.

```shell
$ git add <your files>
$ git commit -m "A really thorough explanation of what we did since this is someone else's work."
$ git push origin master
```

Finish what you started working on, then push up any additional commits.

File a pull request with the commits in it that you want to share. Make sure you have a good explanation in the pull request of what this is, what it's intended to do, and some nice language, rather than making fun of the original author.

### How to work on two different things at the same time

Branching is for when you want to work on something that might span over multiple commits, that's significant enough to warrant some kind of really specific deliniation. 

### Typical Collaboration Patterns

A typical collaboration pattern is actually to fork, then branch off of master, then push to your fork, then file a pull request.

The reason for this is that master, as a branch, should always represent code or whatever that "Works" and is uitable for deployment or sharing or whatever "going public" is for you.

### Creating Aliases To Make Things Simpler

In order to simplify git commands for the lazy people and if you don't want to type out the entire command such as checkout or status then the following is the way to do it:
$ git config --global alias.<whatever you want it to be> <command>

These are my aliases for the following commands for future reference.

```shell
$ git config --global alias.ch checkout
$ git config --global alias.br branch
$ git config --global alias.com commit
$ git config --global alias.st status
```
