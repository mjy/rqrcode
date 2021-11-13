# frozen_string_literal: true

require 'bundler/gem_tasks'
require 'rspec/core/rake_task'
require 'rake/dsl_definition'
require 'rake'
require 'rspec'

RSpec::Core::RakeTask.new(:spec) do |rspec|
  rspec.pattern = FileList['spec/**/*_spec.rb']
end

task default: %i[spec]

desc 'open an irb session preloaded with this gem'
task :console do
  sh 'irb -r pp -r ./lib/rqrcode.rb'
end
