# Cookiecutter template - SAM GO Lambda

## Install golang
Template creates a golang project that expects gomodules.  So you will need 1.11 incase you already have go installed

<a href="https://golang.org/dl/">Official Installation guidelines</a>

## Install sam

<a href="https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/serverless-sam-cli-install.html">Official Installation Guidelines</a>

or

```text
brew upgrade
brew update
brew tap aws/tap
brew install aws-sam-cli
```

## Create new project

```text
sam init -l  https://github.com/basketsavings/sam-lambda-go.git -o $GOPATH/src/github.com/basketsavings
#prompt for project_name
#prompt for base_path


```

For example

```text
sam init -l https://github.com/basketsavings/sam-lambda-go.git -o $HOME/go/src/github.com/basketsavings
# project_name: my-test
# base_path: base path mapping to core api
```

You only need to specify the full git url the first time you use the template.  Subsequent times can be done simply as ```sam-lambda-go```.

```text
sam init -l sam-lambda-go -o $HOME/go/src/github.com/basketsavings
...
```

Unless of course you want the latest changes to the template...in which case use the full git url

## Open project

```text
cd $HOME/go/src/github.com/basketsavings/my-test
code .
```

## Running the project

Follow instructions in the readme of the newly created project