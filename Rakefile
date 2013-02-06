task :default => [:install]

task :install do
  Dir.glob('.*') { |f| FileUtils.cp(f, `echo $HOME`.strip, verbose: true) if f != '.' && f != '..' && f != '.git' }
end
