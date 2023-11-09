# form

## hidden tag

```erb
<%= form_with(url: 'some_path') do |form| %>
  <%= form.hidden_field(:id, value: 123) %>
<%= end
```
