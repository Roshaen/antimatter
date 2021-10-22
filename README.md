[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Open Source Love svg1](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)

<h1 align = "center">Antimatter 🚀</h1>

<p align="center">
  <img width="460" height="400" src="https://user-images.githubusercontent.com/48213106/135222784-5486e9e1-7c23-4e2e-af60-3f1782b70e9c.png">
</p>
<br>

# This is an ELT and analytics project

<a target="_blank" rel="noopener" href="https://antimatter-hackstrap.gitbook.io/antimatter/">Documentation</a>

# 🚀 CONTRIBUTING GUIDELINES

This project aims to simplify Modern ETL and Data Analytics Engine

## Fork this repository

Fork this repository by clicking on the fork button on the top of this page.
This will create a copy of this repository in your account.

## Clone the repository

Now clone the forked repository to your machine. Go to your GitHub account, open the forked repository, click on the code button and then click the _copy to clipboard_ icon.

Open a terminal and run the following git command:

```
git clone "url you just copied"
```

where "url you just copied" (without the quotation marks) is the url to this repository (your fork of this project). See the previous steps to obtain the url.

For example:

```
git clone https://github.com/YOUR-USERNAME/antimatter.git
```

where `YOUR-USERNAME` is your GitHub username. Here you're copying the contents of the first-contributions repository on GitHub to your computer.

## Create a branch

Change to the repository directory on your computer (if you are not already there):

```
Run `cd antimatter`

```

Now create a branch using the `git checkout` command:

```
Run `git checkout <BRANCH_NAME>`

```

For example:

```
git checkout -b backend
```

## Make necessary changes and commit those changes

If you go to the project directory and execute the command `git status`, you'll see there are changes.

Add those changes to the branch you just created using the `git add` command:

```
git add .
```

Now commit those changes using the `git commit` command:

```
git commit -m "Add <your-name> to the repository"
```

replacing `<your-name>` with your name.

## Push changes to GitHub

Push your changes using the command `git push`:

```
git push origin <add-your-branch-name>
```

replacing `<add-your-branch-name>` with the name of the branch you created earlier.

## Submit your changes for review

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

## Getting started with the applications

> **Note:** You need a linux environment to run this application.

First build the react app by running the below command

`docker compose build antimatter`

Now you can individually build each service one by one

`docker compose up --no-deps clickhouse`

`docker compose up --no-deps redis jitsu`

> **Note:** You need to run chmod to give the necessary folder access to jitsu.

`docker compose up --no-deps sqlpad`

`docker compose up --no-deps trino`

`docker compose up --no-deps cube`

`docker compose up --no-deps metabase`

Now access the antimatter application on http://localhost:3000

# 🔗 Links

- <a target="_blank" rel="noopener" href="http://localhost:8123/play">Clickhouse</a>
- <a target="_blank" rel="noopener" href="http://localhost:8001/configurator">Jitsu</a>
- <a target="_blank" rel="noopener" href="http://localhost:3000">SQLPad</a>
- <a target="_blank" rel="noopener" href="http://localhost:4000/#/connection">Cube.js</a>
- <a target="_blank" rel="noopener" href="http://localhost:8080/ui/login.html">Trino</a>
- <a target="_blank" rel="noopener" href="http://localhost:3001/">Metabase</a>

> **Note:** A minimum of 16GB RAM is required to start all the services at once. Insufficient RAM could result in crashing of the Docker daemon.
