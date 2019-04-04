Clone the project
bundle install
./bin/puma
see the stack_trace

```
ylecuyer@hawk:~/Projects/bugged-puma-plugin$ ./bin/puma -p 5000
* Pruning Bundler environment
Traceback (most recent call last):
	15: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/bin/puma-wild:29:in `<main>'
	14: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/bin/puma-wild:29:in `new'
	13: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/cli.rb:71:in `initialize'
	12: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/cli.rb:71:in `new'
	11: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/launcher.rb:61:in `initialize'
	10: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/configuration.rb:194:in `load'
	 9: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/configuration.rb:194:in `each'
	 8: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/configuration.rb:194:in `block in load'
	 7: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/dsl.rb:43:in `_load_from'
	 6: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/dsl.rb:43:in `instance_eval'
	 5: from config/puma.rb:1:in `_load_from'
	 4: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/dsl.rb:79:in `plugin'
	 3: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/configuration.rb:274:in `load_plugin'
	 2: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/plugin.rb:12:in `create'
	 1: from /home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/plugin.rb:47:in `find'
/home/ylecuyer/.rbenv/versions/2.5.3/lib/ruby/gems/2.5.0/gems/puma-3.12.1/lib/puma/plugin.rb:50:in `rescue in find': Unable to find plugin: heroku (Puma::UnknownPlugin)
```
