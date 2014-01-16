---
layout: post
title: "错误：Could not locate Gemfile"
---

现象：
- rails命令执行的时候总不是最新版本
- compass命令执行报错

```
.rvm/gems/ruby-2.0.0-p247@global/gems/bundler-1.3.4/lib/bundler/shared_helpers.rb:22:in `default_gemfile': Could not locate Gemfile (Bundler::GemfileNotFound)
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247@global/gems/bundler-1.3.4/lib/bundler.rb:231:in `default_gemfile'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247@global/gems/bundler-1.3.4/lib/bundler.rb:177:in `root'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247@global/gems/bundler-1.3.4/lib/bundler.rb:99:in `bundle_path'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247@global/gems/bundler-1.3.4/lib/bundler.rb:351:in `configure_gem_home_and_path'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247@global/gems/bundler-1.3.4/lib/bundler.rb:90:in `configure'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247@global/gems/bundler-1.3.4/lib/bundler.rb:146:in `definition'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247@global/gems/bundler-1.3.4/lib/bundler.rb:116:in `setup'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247@global/gems/bundler-1.3.4/lib/bundler.rb:132:in `require'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247/gems/compass-0.13.alpha.0/bin/compass:25:in `<top (required)>'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247/bin/compass:23:in `load'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247/bin/compass:23:in `<main>'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247/bin/ruby_noexec_wrapper:14:in `eval'
        from /Users/zouhaisong/.rvm/gems/ruby-2.0.0-p247/bin/ruby_noexec_wrapper:14:in `<main>'
```
执行 rubygems-bundler-uninstaller 以后就好了
参见http://stackoverflow.com/questions/10610254/cant-install-compass-via-rvm

