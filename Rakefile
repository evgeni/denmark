$:.unshift File.expand_path("../lib", __FILE__)
require 'denmark/version'
require 'bundler/gem_tasks'
require 'github_changelog_generator/task'

task :default do
  system("rake -T")
end

GitHubChangelogGenerator::RakeTask.new :changelog do |config|
  config.user = 'binford2k'
  config.project = 'denmark'
  config.future_release = Denmark::VERSION
end
