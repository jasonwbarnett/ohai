source "https://rubygems.org"

gemspec

gem "chef-config", git: "https://github.com/chef/chef", glob: "chef-config/chef-config.gemspec"
gem "chef-utils", git: "https://github.com/chef/chef", glob: "chef-utils/chef-utils.gemspec"

# NOTE: do not submit PRs to add pry as a dep, add to your Gemfile.local
group :development do
  gem "chefstyle", git: "https://github.com/chef/chefstyle.git", branch: "master"
  gem "ipaddr_extensions"
  gem "rake", ">= 10.1.0"
  gem "rspec-collection_matchers", "~> 1.0"
  gem "rspec-core", "~> 3.0"
  gem "rspec-expectations", "~> 3.0"
  gem "rspec-mocks", "~> 3.0"
  gem "rubocop-performance", "1.8.0"
  gem "rubocop-rspec"
end

group :docs do
  gem "github-markup"
  gem "redcarpet"
  gem "yard"
end

group :debug do
  gem "pry"
  gem "pry-byebug"
  gem "pry-stack_explorer", "~> 0.4.0" # pin until we drop ruby < 2.6
  gem "rb-readline"
end
