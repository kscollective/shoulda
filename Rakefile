require 'rubygems'
require 'bundler/gem_tasks'
require 'cucumber/rake/task'

desc "Clean files generated by rake tasks"
task :clobber => [:clobber_rdoc, :clobber_package]

Cucumber::Rake::Task.new do |t|
  t.fork = true
  t.cucumber_opts = ['--format', (ENV['CUCUMBER_FORMAT'] || 'progress')]
end

desc 'Default: run cucumber features'
task :default => [:cucumber]
