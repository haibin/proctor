## Proctor

Proctor is a developer friendly automation orchestrator. It helps everyone use automation and contribute to it

### proctor CLI

Proctor CLI is a command line tool to interact with [proctord](#)
Users can use it to run procs

### Dev environment setup

* Install and setup golang
* Install glide
* Make a directory `src/github.com/gojektech` inside your GOPATH
* Clone this repo inside above directory
* Install dependencies using glide
* [Configure proctor CLI](#proctor-cli-configuration)
* Running `go install github.com/gojektech/proctor` will place the CLI binary in your `$GOPATH/bin` directory
* Run `proctor version` to check installation

### Running tests instructions

* [Setup dev environment](#dev-environment-setup)
* Run tests: `go test -race -cover $(glide novendor)`

#### Proctor CLI configuration

* Make a directory `.proctor` inside your home directory
* Create a file proctor.yaml inside above directory
* Put the following content in the above file

```
PROCTOR_URL: [URL to proctor Engine]
```
