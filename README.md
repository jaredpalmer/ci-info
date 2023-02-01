# `ci-info`

A partial Go port of https://github.com/watson/ci-info


## Install

```sh
go get github.com/jaredpalmer/ci-info
```

## Usage

```go
package main

import "github.com/jaredpalmer/ci-info"

func main() {
  fmt.Println(ci.IsCi()) // true or false 
  fmt.Println(ci.Name()) // => (e.g. nil, "Vercel", "CircleCI" etc.
  fmt.Println(ci.Info())  // { Name:     "CircleCI", Constant: "CIRCLE", Env:      "CIRCLECI" },
}
```

## Providers

This package can detect the following CI/CD/PaaS providers:

- AppVeyor
- Azure Pipelines
- Appcircle
- Bamboo
- Bitbucket Pipelines
- Bitrise
- Buddy
- Buildkite
- CircleCI
- Cirrus CI
- AWS CodeBuild
- Codefresh
- Codeship
- Drone
- dsari
- GitHub Actions
- GitLab CI
- GoCD
- LayerCI
- Hudson
- Jenkins
- Jenkins
- Magnum CI
- Netlify CI
- Nevercode
- Render
- Sail CI
- Semaphore
- Screwdriver
- Shippable
- Solano CI
- Strider CD
- TaskCluster
- TeamCity
- Travis CI
- Vercel
- Visual Studio App Center

