task :default => [:install]

task :install do
  home = `echo $HOME`.strip
  Dir.glob( '.*' ) do |f|
    if f != '.' && f != '..' && f != '.git' && f != '.DS_Store'
      FileUtils.cp( f, home, verbose: true )
    end
  end

  FileUtils.cp( 'install-deps.sh', home, verbose: true )
end
