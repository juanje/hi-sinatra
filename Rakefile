require 'rake'
require 'cucumber'
require 'cucumber/rake/task'

desc 'run the app'
task :run do |t|
  load 'lib/app.rb'
  App.run!
end

desc 'run cucumber features'
Cucumber::Rake::Task.new(:features) do |t|
  t.cucumber_opts = 'features --format pretty'
end

task :default => :run
