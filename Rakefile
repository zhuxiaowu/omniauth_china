require 'rubygems'
require 'bundler'
Bundler.setup
require 'rake'

require 'mg'
MG.new('omniauth_china.gemspec')

require 'rspec/core/rake_task'
RSpec::Core::RakeTask.new(:spec) do |s|
  s.rspec_opts = "--format=#{ENV['RSPEC_FORMAT'] || 'nested'} --colour"
end

task :default => :spec
