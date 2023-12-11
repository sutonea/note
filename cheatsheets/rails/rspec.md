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

## array

### test order

**書式**
```ruby
.to match([a, b, c])
```

**例**

```ruby
expect([1, 2, 3]).to match [1, 2, 3]
```
