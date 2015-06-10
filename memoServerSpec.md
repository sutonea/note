# serverspec の導入

参考: http://serverspec.org/

## 前提条件

rbenv 導入済み

`~/work/` 作成済

## 作業の記録

```
cd ~/work
mkdir ruby_system_gem
cd ruby_system_gem/
rbenv shell system
echo "source 'https://rubygems.org'" >> Gemfile
echo "gem 'serverspec'" >> Gemfile
```

メッセージが表示された。systemのrubyにはbundlerが入っていなかった
```
rbenv: bundle: command not found

The `bundle' command exists in these Ruby versions:
  2.1.1
  2.2.1
```

```
rbenv shell 2.2.1
bundle
```

インストール完了
```
Bundle complete! 1 Gemfile dependency, 13 gems now installed.
Use `bundle show [gemname]` to see where a bundled gem is installed.
```


## serverspec を実行

`serverspec-init` では command not found となってしまった

```
rbenv exec serverspec-init
```

上記コマンド実行後、ウィザードは公式サイト通りに実行
