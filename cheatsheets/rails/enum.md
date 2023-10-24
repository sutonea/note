# Rails enum チートシート


```ruby
class MyClass
  enum status: { default: 0, public: 1, private: 2 }
end
```

```ruby
MyClass.statuses # => { "default" => 0, "public" => 1, "private" => 2 }
MyClass.statuses[:public] # => 1
MyClass.statuses["private"] # => 2
```
