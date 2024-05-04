# Add your own tasks in files placed in lib/tasks ending in .rake,
# for example lib/tasks/capistrano.rake, and they will automatically be available to Rake.

require_relative "config/application"

Rails.application.load_tasks


namespace :secrets do
    desc "Generate a unique secret key"
    task :generate do
      puts SecureRandom.hex(64)
    end
  end
  