# pry
> debug with pry.

## install
```rb
gem 'pry-rails', group: [:development, :test]
gem 'pry-byebug', group: [:development, :test]

## OR
group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug'
  gem 'pry-byebug'
  gem 'pry-rails'
end
```

## Add debugger:
```html
<% binding.pry %>
```

## debug in ruby:
```rb
binding.pry
```
