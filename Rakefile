require 'fileutils'

task :clean do
  FileUtils.rm_rf 'dist'
end

desc 'compile the swf file'
task :swf => :clean do
  FileUtils.mkdir_p 'dist'
  `mtasc -cp src Jplayer.as -swf dist/Jplayer.swf -main -header 600:120:40 -v -version 8 -group`
end