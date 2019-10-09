# Jimbos First Serverless Go Lang Lambda
An example of an AWS Lambda function written in Go!

## Motivation
I went to serverlessconf 2019 today and met lots of people who are already writing lambda fuctions in go- whaaaaat! I had to get in on the fun so I went over into a corner and used the serverless framework to scaffold out a fresh go lang lambda function: 

```
serverless create -t aws-go-dep -p jimbos-go-lang-lambda
```
...and just that that I had a go lang lambda function!

## Usage

Once you have cloned this project, you just navigate into the project directory and run `make`:
```
cd jimbos-go-lang-lambda
```
```
make
```

### Potential Snags

#### dep: No such file or directory

Initially, I was getting this error when running `make`:
```
dep ensure -v
make: dep: No such file or directory
make: *** [build] Error 1
```

To Fix: I needed to install (dep)[https://github.com/golang/dep]:
```
brew install dep
brew upgrade dep
```

#### is not within a known GOPATH/src

/Users/loaner/Git-Projects/Jimbos-Serverless-Go-Lang-Lambda/jimbos-go-lang-lambda is not within a known GOPATH/src
make: *** [build] Error 1

To Fix: ? lol
