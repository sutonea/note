# Validate

## uniq

```ruby
validates :email, uniqueness: true
```

with other column

```ruby
validates :name, uniqueness: { scope: :year }
```

```ruby
validates :name, uniqueness: { scope: :year,
    message: "Some error message" }
```
