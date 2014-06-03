# -*- coding: UTF-8 -*-
require 'rspec/core/rake_task'
require 'rubocop/rake_task'

RSpec::Core::RakeTask.new(:spec)

RuboCop::RakeTask.new(:rubocop) do |t|
  t.patterns =
    %w( Rakefile Gemfile skel.gemspec lib/**/*.rb spec/*_spec.rb )
  t.fail_on_error = true
end

task default: [:rubocop, :spec]
