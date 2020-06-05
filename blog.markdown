---
title: blog
date: 2020-06-04 18:15:00 Z
author: Janvier Byiringiro
layout: default
---


Why StackOverflow?
StackOverflow has been around for many years and it has been really a powerful tool for my every technical role. So i decide to make this site available for my use in terminal. For my current role I get to work with server Maintenance, Monitoring and Backup. This will be a great search tool when working with remote servers and you don't have to open a browser to search for errors fix ideas.

Finished Tool: https://github.com/jenzzly/jenzzly

1. Stack Overflow API customization
You will need to customize your search to your liking on this ' https://api.stackexchang.com/docs/answers' remember there is a limit on how much to hit the request.

Example: https://api.stackexchange.com/2.2/answers?order=desc&sort=activity&site=stackoverflow

2. Ruby Script
Here is my ruby script but remember your can write your own as well and change however you want it.

GitHub logo jenzzly / jenzzly
Search on stack overflow script
Jenzzly
Welcome to jenzzly gem, This scripts help do search on stackoverflow thru command line.

Installation
Add this line to your application's Gemfile:

gem 'jenzzly'
And then execute:

$ bundle install
Or install it yourself as:

$ gem install jenzzly
Usage
Once done with Installation $jenzzly Your_search_key_word

Development
After checking out the repo, run bin/setup to install dependencies. You can also run bin/console for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run bundle exec rake install. To release a new version, update the version number in version.rb, and then run bundle exec rake release, which will create a git tag for the version, push git commits and tags, and push the .gem file to rubygems.org.

Contributing
Bug reports and pull requests are welcome on GitHub at https://github.com/jenzzly/jenzzly.

License
The gem is available as…

View on GitHub
3. Publish as Gem CLI
I chose to publish as gem mostly because it was easier and I like ruby anyway. For creating a gem please follow this repo below.

How-to Create a Ruby CLI Gem
Pre-Setup
Create a RubyGems Account
Install RVM (Ruby Version Manager) : RVM
Install Bundler: gem install bundler
Project Creation
Navigate to the parent directory you want to create your gem repository directory in.
Create Gemset: rvm gemset create yourGemName
Use Gemset: rvm gemset use yourGemName
Bundle Gem: bundle gem yourGemName
Open the app's parent file located at lib/yourGemName.rb
Create a Hello World output
require "yourGemName/version"

module yourGemName
  class Test
    def say_hello
      puts "Hello World!"
    end
  end
end
Create an executable file at bin/yourGemName (no file extension)
Add Shebang #!/usr/bin/env ruby and code to call your Hello World output
#!/usr/bin/env ruby

require 'yourGemName'

test = yourGemName::Test.new
test.say_hello
Create a CHANGELOG.md file in the project directory
Create repository on Github
Make initial commit: git commit -m "Initial commit"
Push code to repository on Github:
git remote add origin git@github.com:yourusername/yourGemRepo.git
git push -u origin master
Open gemspec - /yourGemName.gemspec
Update todo lines:
Update spec.summary
Update spec.descriptions
Update spec.homepage
Update spec.metadata["source_code_uri"] (Github Repo Page)
Update spec.metadata["changelog_uri"] (Github CHANGELOG.md link)
Update spec.bindir to bin
Update spec.executeables to yourGemName (the file in /bin)
Run Bundle Install: bundle install
Build Binary: rake install
Test output: yourGemName --> "Hello World"
Deploying Gem
Commit Changes to Github
Build Gem: gem build yourGemName
Push Gem to RubyGems.org: gem push yourGemName-0.1.0.gem
view rawruby-cli-gem.md hosted with ❤ by GitHub

4. Usage
Once done with Installation you can use your new tool like this: Mine is called "jenzzly" and my search will be
"jenzzly your_key_word_search_text".

Alt Text

Results
Alt Text