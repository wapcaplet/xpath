require 'rubygems'
require 'rspec/core/rake_task'
require 'yard'

desc "Run all examples"
RSpec::Core::RakeTask.new(:spec) do |t|
  #t.rspec_path = 'bin/rspec'
  t.rspec_opts = %w[--color]
end

YARD::Rake::YardocTask.new do |t|
  t.files   = ['lib/**/*.rb', 'README.rdoc']
  t.options = ['--markup', 'markdown']
end

task :default => :spec
