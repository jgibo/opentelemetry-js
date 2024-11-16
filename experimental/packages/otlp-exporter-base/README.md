# OpenTelemetry Collector Exporter for web and node

## Fork Changes

This is a fork of the upstream. The fork adds fetch support into exporter-trace-otlp-http and supporting packages. The fork repo is https://github.com/jgibo/opentelemetry-js, branch service-worker-support. The changes were originally authored by https://github.com/sugi in his fork https://github.com/sugi/opentelemetry-js.

Fetch support is automatically detected by the exporter, and chosen if xhr and beacon are not availeable in the environment (which is the case in a service worker), no changes are required to application code.

Note, the most recent merge of upstream main into service-worker-support branch was on Feb 11 2024, so this change is likely missing a few updates that have been released to the upstream since then.

[![NPM Published Version][npm-img]][npm-url]
[![Apache License][license-image]][license-image]

**Note: This package is intended for internal use only.**

**Note: This is an experimental package under active development. New releases may include breaking changes.**

This module provides a base exporter for web and node to be used with [opentelemetry-collector][opentelemetry-collector-url].

## Installation

```bash
npm install --save @opentelemetry/otlp-exporter-base
```

## GRPC

For GRPC please check [npm-url-grpc]

## PROTOBUF

For PROTOBUF please check [npm-url-proto]

## Useful links

- For more information on OpenTelemetry, visit: <https://opentelemetry.io/>
- For more about OpenTelemetry JavaScript: <https://github.com/open-telemetry/opentelemetry-js>
- For help or feedback on this project, join us in [GitHub Discussions][discussions-url]

## License

Apache 2.0 - See [LICENSE][license-url] for more information.

[discussions-url]: https://github.com/open-telemetry/opentelemetry-js/discussions
[license-url]: https://github.com/open-telemetry/opentelemetry-js/blob/main/LICENSE
[license-image]: https://img.shields.io/badge/license-Apache_2.0-green.svg?style=flat
[npm-url]: https://www.npmjs.com/package/@opentelemetry/otlp-exporter-base
[npm-url-grpc]: https://www.npmjs.com/package/@opentelemetry/otlp-grpc-exporter-base
[npm-url-proto]: https://www.npmjs.com/package/@opentelemetry/otlp-proto-exporter-base
[npm-img]: https://badge.fury.io/js/%40opentelemetry%2Fotlp-exporter-base.svg
[opentelemetry-collector-url]: https://github.com/open-telemetry/opentelemetry-collector
