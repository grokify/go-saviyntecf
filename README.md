# Saviynt External Connector Framework (ECF) in Go

[![Build Status][build-status-svg]][build-status-url]
[![Go Report Card][goreport-svg]][goreport-url]
[![Docs][docs-godoc-svg]][docs-godoc-url]
[![License][license-svg]][license-url]

This is the Saviynt External Connector Framework (ECF) implemented in Go with Chi.

It is built with [`oapi-codegen)`](https://github.com/deepmap/oapi-codegen).

## Rebuild

To rebuild this module using an updated OpenAPI spec, do the following:

```
% curl -XGET https://raw.githubusercontent.com/saviynt/ExternalConnectorFramework-APISpec/main/spec/OpenAPISpec.yaml > openapi.yaml
% go generate
```

This will create a new `server.gen.go` file using the config at `oapi-codegen.yaml`.

For more information on `oapi-codegen`, see the following:

1. [https://www.jvt.me/posts/2022/07/12/go-openapi-server/](https://www.jvt.me/posts/2022/07/12/go-openapi-server/)

 [used-by-svg]: https://sourcegraph.com/github.com/grokify/go-saviyntecf/-/badge.svg
 [used-by-url]: https://sourcegraph.com/github.com/grokify/go-saviyntecf?badge
 [build-status-svg]: https://github.com/grokify/go-saviyntecf/workflows/test/badge.svg
 [build-status-url]: https://github.com/grokify/go-saviyntecf/actions/workflows/test.yaml
 [goreport-svg]: https://goreportcard.com/badge/github.com/grokify/go-saviyntecf
 [goreport-url]: https://goreportcard.com/report/github.com/grokify/go-saviyntecf
 [codeclimate-status-svg]: https://codeclimate.com/github/grokify/go-saviyntecf/badges/gpa.svg
 [codeclimate-status-url]: https://codeclimate.com/github/grokify/go-saviyntecf
 [docs-godoc-svg]: https://pkg.go.dev/badge/github.com/grokify/go-saviyntecf
 [docs-godoc-url]: https://pkg.go.dev/github.com/grokify/go-saviyntecf
 [loc-svg]: https://tokei.rs/b1/github/grokify/go-saviyntecf
 [repo-url]: https://github.com/grokify/go-saviyntecf
 [license-svg]: https://img.shields.io/badge/license-MIT-blue.svg
 [license-url]: https://github.com/grokify/go-saviyntecf/blob/master/LICENSE
