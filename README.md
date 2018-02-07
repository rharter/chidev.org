# chidev.org

This repository contains the Jekyll project that is used to build [chidev.org](http://chidev.org/).

## Local Development

In order to develop against the site locally, you'll need to install:

- Ruby
- Bundler

Once those are installed, install the Ruby specific dependencies:

```bash
$ bundle
```

After that, you should be able to use `jekyll serve` to view changes [locally](http://localhost:9000/) as you make them.

## Deployment

Deployment is handled automatically by [Travis CI](https://travis-ci.org/rharter/chidev.org) on merges to `master`. The deployment process writes to an [Amazon S3](http://aws.amazon.com/s3/) bucket that is configured to serve static website content. The DNS for that bucket is handled by [Route 53](http://aws.amazon.com/route53/).

Check [.travis.yml](.travis.yml) for more detail.
