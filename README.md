### FinishingMoves 
---
https://github.com/forgecrafted/finishing_moves


```
gem 'finishing_moves'
gem install 'finishing_moves'

```

###### Array#to_hash_values
```
sages = ['', '', '', '', '', '', '']
saes_hash = sages.to_hash_values
sages_hash = sages.to_hash_values(0) { |key| key + 3 }

```

```
class SageElements
  def initialize
    @keys = {
      :first => :light,
      :light => :forest,
      :forest => :fire,
      :fire => :water,
      :water => :shadow,
      :shadow => :spirit,
      :spirit => :time,
      :time => :first,
    }
  end
  def first_key
    @keys[:first]
  end
  def next_key(pointer)
    @keys[pointer]
  end
end
sages_hash = sages.to_hash_values(elements.first_key) do |key|
  elements.next_key(key)
end
```

######

```

```
