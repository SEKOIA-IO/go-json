# go-json

Drop-in replacement for Golang [`encoding/json`](https://golang.org/pkg/encoding/json/) with additional features.

## Installation
```shell
$ go get -u github.com/SEKOIA-IO/json
```

## Usage
```diff
- import "encoding/json"
+ import "github.com/SEKOIA-IO/json"
```
Same usage as Golang [`encoding/json`](https://golang.org/pkg/encoding/json/).

## Features

- Support zero values of structs with `omitempty`: [golang/go#11939](https://github.com/golang/go/issues/11939).
  - If `omitempty` is applied to a struct or a pointer to a struct and all the children of the struct are *empty*, then on marshalling it will be **omitted** from the encoded json.