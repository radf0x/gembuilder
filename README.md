# gembuilder
A gem to generate the scaffolding of another gem <br>
take laziness to another level because why not?

### How to use
1. `$ ./gembuilder [your desired gem name]`
2. Follow instructions on screen <br>
![demo](https://media.giphy.com/media/j3KI7xkA3TBOfxsjmK/giphy.gif)

### What will it generates?
1. A folder with files below:
```
no-scope
├── no-scope.gemspec
└── lib
    └── no-scope.rb
```
2. A empty class with camelcase gem_name (/lib/no-scope.rb)
```ruby
# frozen_string_literal: true

class NoScope

end
```
3. A default gemspec with TODOs
```ruby
Gem::Specification.new do |s|
  s.name        = "<%= no-scope %>"   
  s.version     = '0.0.1'   
  s.summary     = "<%= no-scope %>"   
  s.description = "[TODO]"   
  s.authors     = [""]   
  s.email       = ''
  s.files       = ["lib/<%= no-scope %>.rb"]   
  s.homepage    = "[TODO]"   
  s.license     = "<%= @license %>"
end
```
### TODO
1. Support different format for gem_name input
2. Add standard methods on the new gem main class
3. Not sure if im going to work on this lib anytime soon but <b>look!</b> <br>A lazy cat is having a nap on the couch<br>
![cat](https://media.giphy.com/media/pVkmGyqYRt4qY/giphy.gif)