# docker-opsweekly Rakefile to standardize commands

desc "Build the docker image"
task :build do
  sh "docker build -t backln/opsweekly ."
end

desc "Run the docker image"
task :run do
  sh "docker run -e MYSQL_ROOT_PASSWORD=password -it backln/opsweekly"
end

desc "Debug the docker image by running but with a shell, not the default cmd"
task :debug do
  sh "docker run -e MYSQL_ROOT_PASSWORD=password -e OPSWEEKLY_MYSQL_PASSWORD=opsweekly --entrypoint /bin/bash -it backln/opsweekly"
end