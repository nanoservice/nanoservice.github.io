---
layout: landing
title: "nanoservice project home page"
comments: true
sharing: true
footer: true
---

Open source set of tools, systems and libraries to let developers build and
deploy fully asynchronous nanoservices with ease.

### * Fast to setup

### * Easy to use

### * Pleasure to deploy

## Install & Configure

```bash
curl -L https://github.com/nanoservice/installer/raw/stable/install.sh | bash

# configure nanoservice cluster on AWS (credentials, DNS, etc)
nanoservice configure

# or configure hosted nanoservice cluster with your credentials
nanoservice configure --hosted

# or configure local docker cluster for development
nanoservice configure --docker
```

## Build your first "Hello world" web-nanoservice

```bash
nanoservice create helloworld --web --golang
cd helloworld/
```

Edit `main.go`:

```go
package main

import "github.com/nanoservice/libs-go/web"

func main() {
  web.Route("/", func(w *web.Response, r *web.Request) {
    // this is actually the only line we modified here
    w.Println("Hello, world!")
  })
  web.Start()
}
```

And deploy your app:

```bash
nanoservice deploy
```

Now if you reach http://helloworld.nanoservice.yourdomain.com/, you will see
`Hello, world!` response. By the way, if you reach `/health` path, you will get
`OK` - this is built-in health check mechanism.

## What next?

* [Tutorials](/tutorials)
* [Examples](/examples)
* [Documentation](/docs)
