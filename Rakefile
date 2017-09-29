# require 'jekyll/test/tasks'
# task default: "jekyll:check"

task :build => ["build:prod"]
namespace :build do

  desc "Regenerate files for production"
  task :prod do
    puts "* Regenerating files for production... first time"
    system "bundle exec jekyll build"
    puts "* Finish"
  end

  desc "Regenerate files for development"
  task :dev do
    puts "* Generating files for development..."
    system "bundle exec jekyll serve -L --limit_posts 5 --incremental --profile --config _config.yml,_config_dev.yml --profile"
  end

end
