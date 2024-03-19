# Usage

```ruby
class MyClass
  extend ActiveSupport::Concern
end
```

# included

```ruby
class MyClass < ApplicationRecord
  extend ActiveSupport::Concern

  def included do
    belongs_to :some_model
  end
end
```
