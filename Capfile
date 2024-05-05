# Load DSL and set up stages
require "capistrano/setup"

# Include default deployment tasks
require "capistrano/deploy"
require "capistrano/rvm"

# Load the SCM plugin appropriate to your project (e.g., Git)
require "capistrano/scm/git"
install_plugin Capistrano::SCM::Git

# Include Puma-related tasks
require "capistrano/puma"
install_plugin Capistrano::Puma
install_plugin Capistrano::Puma::Daemon

# Include other gems/tasks as needed (e.g., bundler, rails)
require "capistrano/bundler"
require "capistrano/rails/assets"
require "capistrano/rails/migrations"

# Load custom tasks from `lib/capistrano/tasks` if you have any defined
Dir.glob("lib/capistrano/tasks/*.rake").each { |r| import r }
