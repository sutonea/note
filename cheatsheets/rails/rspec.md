# matcher

## raise error

**書式**
```ruby
.to raise_error(<Error type>)
```

**例**
```ruby
expect { some_method }.to raise_error(ActiveRecord::RecordInvalid)
```
