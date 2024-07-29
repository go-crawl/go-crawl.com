+++
title = 'Command line tool'
date = 2024-07-29T18:58:15+02:00
draft = false
+++

## Default structure of Gocrawl projects

```
gocrawl.cfg
myproject/
    items.go
    middlewares.go
    pipelines.go
    settings.go
    spiders/
        spider1.go
        spider2.go
        ...
```
The directory where the gocrawl.cfg file resides is known as the project root directory. That file contains the name of the golang module that defines the project settings. Here is an example:

```ini
[settings]
default = myproject.settings
```

## Using the gocrawl tool

### Creating projects

The first thing you typically do with the gocrawl tool is create your Gocrawl project:

```bash
gocrawl startproject myproject [project_dir]
```
That will create a Gocrawl project under the project_dir directory. If project_dir wasn’t specified, project_dir will be the same as myproject.

Next, you go inside the new project directory:

cd project_dir
And you’re ready to use the gocrawl command to manage and control your project from there.