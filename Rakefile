# launch the application via bundle exec rackup 3000 0.0.0.0
desc "Run the app"
task :run do
  sh "bundle exec rackup -p 3000 -o 0.0.0.0"
end

desc "Run the sample lib file"
task :run_gpt3_sample do
  sh "bundle exec ruby ./lib/gpt3_answer_bot.rb"
end

desc "Publish - publish docker containers"
task :publish do
  sh "docker-compose build && docker-compose push"
end

# TODO: remove
task :refresh do
  sh "cd ~/apps/makevoid-docker && rake"
end

task default: :run
