# Where is my weekend?

## Installation

```ruby
gem 'where_is_my_weekend'
```

## How to use

```ruby
dates = [Time.new(2016, 12, 23), Time.new(2016, 12, 24), Time.new(2016, 12, 25), Time.new(2016, 12, 26)]
# => [2016-12-23 00:00:00 -0200, 2016-12-24 00:00:00 -0200, 2016-12-25 00:00:00 -0200, 2016-12-26 00:00:00 -0200]
```

- `weekend_day?` will return `true` if a date is a weekend day

```ruby
dates.first.weekend_day?
# => false

dates.second.weekend_day?
# => true
```

- `any_weekend?` will return `true` if on a array of dates have any weekend day

```ruby
dates.any_weekend?
# => true
```

- `weekend_dates` will return a array of weekend days from a array of dates

```ruby
dates.weekend_dates
# => [2016-12-24 00:00:00 -0200, 2016-12-25 00:00:00 -0200]
```
