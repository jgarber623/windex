require "rake"
require "erb"

task :default => :install

desc "Install .htaccess file for Windex."
task :install do
  puts "Where is your local web root? (Be sure to include the trailing slash!)"
  sitespath = STDIN.gets.chomp
  system %Q{cp $PWD/main.htaccess #{sitespath}.htaccess}
  system %Q{ln -fs $PWD/windex/ #{sitespath}windex}
end