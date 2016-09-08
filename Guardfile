# frozen_string_literal: true
ignore %r{^ignored/path/}, /public/
filter /\.txt$/, /.*\.zip /

group :unit do
  guard :rspec, :cmd => 'bundle exec rspec --fail-fast' do

    watch(%r{^.+(?<!test)/.+\.rb})  { "spec" }
  end
end
