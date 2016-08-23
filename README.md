# Docker scss-lint

## What is scss-lint

`scss-lint` is a tool to help keep your [SCSS](http://sass-lang.com) files
clean and readable by running it against a collection of
configurable [linter rules](lib/scss_lint/linter/README.md). You can run it
manually from the command line, or integrate it into your
[SCM hooks](https://github.com/brigade/overcommit).

You can get more informations at: [https://github.com/brigade/scss-lint](https://github.com/brigade/scss-lint).

## Run using Docker

```sh
docker run --rm -v $(pwd):/app rvip/scss-lint
```

You can pass in every options scss-lint accepts:

```sh
docker run --rm -v $(pwd):/app rvip/scss-lint src/
```

For the full list of options, go to [scss-lint official README](https://github.com/brigade/scss-lint#usage).

## Build

```sh
git clone https://github.com/ReputationVIP/docker-scss-lint.git && cd docker-scss-lint
docker build -t your-namespace/scss-lint .
```
