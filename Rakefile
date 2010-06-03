#!/usr/bin/env rake

require 'pathname'

desc 'Updates all submodules to their latest version'
task :update do
  Pathname.glob('*.tmbundle') do |bundle|
    Dir.chdir(bundle) do
      `git checkout master`
      `git pull`
    end
  end
end
