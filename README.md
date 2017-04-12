# Instrumental Statsite Sink

Instrumental is a [application monitoring platform](https://instrumentalapp.com) built for developers who want a better understanding of their production software. Powerful tools, like the [Instrumental Query Language](https://instrumentalapp.com/docs/query-language), combined with an exploration-focused interface allow you to get real answers to complex questions, in real-time.

This data sink allows [Statsite](https://github.com/armon/statsite) to send metrics to Instrumental.

## Install

```console
$ gem install statsite-instrumental
```

## Configuration

To use the sink you need to set `stream_cmd` in your config for statsite. Make
sure you're using the correct path to the executable and supply your
instrumental [project API token](https://instrumentalapp.com/docs/tokens) as the only argument to the script.

```
[statsite]
stream_cmd = /usr/local/bin/statsite-instrumental PROJECT_API_TOKEN
```

## Note on Patches/Pull Requests

* Fork the project.
* Add tests to show the problem or test your feature
* Make your feature addition or bug fix.
* Send me a pull request. Bonus points for topic branches.

Please don't make changes to the Rakefile, version, or history.

## Development

```console
$ gem install bundler
$ bundle
$ guard
```

## Copyright

See LICENSE for details.
