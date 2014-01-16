---
layout: post
title: "gem安装的时候不要安装ri和rdoc"
---

修改~/.gemrc,最后增加一行gem: --no-ri --no-rdoc

```
---
:backtrace: false
:benchmark: false
:bulk_threshold: 1000
:sources:
- http://ruby.taobao.org/
:update_sources: true
:verbose: true
gem: --no-ri --no-rdoc
```