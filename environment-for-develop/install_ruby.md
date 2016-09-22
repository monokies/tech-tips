# RubyとRuby on Railsのインストール

## 環境情報

* MacBook Air (Mid 2011)
  * OS X El Capitan

## Rubyの最新バージョンインストール

以下のサイトの情報をそのまま利用した。

* http://qiita.com/keneo/items/1772adc2ebbde229fb71 を参照した

使ったコマンド（後で精査する）

```sh
> brew install ruby
> ruby -v
> cd ~/Downloads/
> ls
> llbrew install ruby-build
> brew install ruby-build
> brew install rbenv
> echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> .bash_profile
> echo 'eval "$(rbenv init -)"' >> .bash_profile
> source .bash_profile
> rbenv install -l
> rbenv versions
> gem
> gem install rails
> gem install bundler
> cd /tmp
> ls
> rails new sample
> cd sample/
> rails g scaffold Twitter tweet:string
> rake db:migrate
> raise server
> rails server
```

参考サイト

http://ruby.studio-kingdom.com/rails/guides/getting_started


