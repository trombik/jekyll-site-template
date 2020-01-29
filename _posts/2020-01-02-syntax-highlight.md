---
lang: en
layout: post
title: Syntax highlight example
tags:
- example

---

YAML example:

```yaml
foo:
  bar: buz
```

Ruby example:

```ruby
class YoutubeTag < Liquid::Tag
  def initialize(tag_name, arg, tokens)
    super # mandatory
    # fill in some awesome codez
  end

  def render(context)
    <<-MARKUP.strip
    # more awesome codez
    MARKUP
  end
end
```
