require 'rake' 
require 'rake/testtask' 
require 'rake/rdoctask' 
require 'jeweler'
 
desc 'Default: run unit tests.' 
task :default => :test 
 
desc 'Test auto_complete plugin.' 
Rake::TestTask.new(:test) do |t| 
  t.libs << 'lib' 
  t.pattern = 'test/**/*_test.rb' 
  t.verbose = true 
end 
 
desc 'Generate documentation for auto_complete plugin.' 
Rake::RDocTask.new(:rdoc) do |rdoc| 
  rdoc.rdoc_dir = 'rdoc' 
  rdoc.title    = 'Auto Complete' 
  rdoc.options << '--line-numbers' << '--inline-source' 
  rdoc.rdoc_files.include('README') 
  rdoc.rdoc_files.include('lib/**/*.rb') 
end

Jeweler::Tasks.new do |gem|
  gem.name = "auto_complete"
  gem.homepage = "https://github.com/rails/auto_complete"
  gem.license = "MIT"
  gem.summary = %Q{Rails auto completion}
  gem.description = %Q{}
  gem.email = ""
  gem.authors = ["David Heinemeier Hansson"]
  gem.extra_rdoc_files = ['README']
  gem.require_paths = ["lib"]
end
Jeweler::RubygemsDotOrgTasks.new
