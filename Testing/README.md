# Testing Standard

List of TMJP Engineering rules &amp; standard workflow in Testing

## Getting Started

In agile, the developers will focus on Test Driven Developement (TDD). TDD is a development technique where you must first write a test that fails before you write new functional code.

### Local

In **Laravel Framework**, we'll be using [phpunit](https://phpunit.de/). **PHPUnit** is a programmer-oriented testing framework for PHP. To run a test, run this command:

```
phpunit
```

In **TMJ Mean Stack** or any javascript application, we'll be using `karma` and `jasmine` together. **Karma** is a test runner for javascript. **Jasmine** is an open source testing framework for javascript. To run a test, run this command:

```
karma
```

### Pull Request

We'll be using CI (Continuous Integration) like [Travis](https://travis-ci.org/) or [CircleCI](https://circleci.com/). For new pu

An example of CI:

![image](https://cloud.githubusercontent.com/assets/21231662/23928718/561170b6-095c-11e7-9be6-51cd3e34b19b.png)

**Travis CI vs Circle CI**

- Travis CI
  - Github integration
  - Free for open source
  - Easy to get started
  - Nice interface
  - Automatic deployment
  - Tutorials for each programming language

- CircleCI
  - Github integration
  - Fast builds
  - Easy setup
  - Competitively priced
  - Slack integration
  - Great customer support

## Credits

[CI Comparison](https://stackshare.io/stackups/travis-ci-vs-circleci-vs-jenkins)
