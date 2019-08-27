---
path: '/phpunit'
title: 'PHPUnit'
github_url: 'https://github.com/pxgamer/phpunit-action'
author: 'Owen Voke'
twitter: '@pxgamer112'
tags: ['php', 'phpunit', 'testing']
subtitle: 'GitHub Action for interacting with PHPUnit.'
---

# Action details

This Action for [PHPUnit](https://phpunit.de) enables arbitrary actions with the PHPUnit command-line client.

## Usage

Via GitHub Workflow

```yml
on: push
name: CI
jobs:
  composer:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v1
      # For YAML Actions, use v1 or later
      - uses: pxgamer/phpunit-action@master
        with:
          # If there isn't a PHPUnit config, specify files or directories to test
          command: tests/
```
