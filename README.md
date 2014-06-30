### rails-app-creator

rails-app-creator is a simple bash script that adds commonly used functionality to a Rails 4 application upon creation. 

To run it, use the command:

	rails-app-creator --name myRailsApp

Options include:

- `--name appName` 
  - Sets application name.  This option is required.  
- `-h or --help`
  - Shows command usage and options.
- `-v or --verbose`
  - Verbose mode.
- `--haml`
  - Adds [haml]() and [haml-rails]() gems.  Also replaces default application layout file with a haml version.
- `--rspec`
  - Adds the [rspec-rails](),[factory_girl_rails](), [faker](), [shoulda-matchers](), [guard-rspec](), and [simplecov]() gems.  Installs RSpec into application.  Alters .rspec file to provide pretty output and require correct config file.  Adds common directories for RSpec tests.  Creates a binstub for RSpec.  Adds RSpec entry to Guardfile.  Adds RSpec to simplecov reports.
- `--cucumber`
  - Adds the [cucumber-rails](), [selenium-webdriver](), [database_cleaner](), [launchy](), and [guard-cucumber]() gems.  Installs Cucumber into application.  Creates binstub for Cucumber. Configures the DatabaseCleaner.  Adds Cucumber entry to Guardfile.  Adds Cucumber to simplecov reports. 
- `--jasmine`
  - Adds the [jasmine-rails](), [jasmine-jquery-rails](), and [guard-jasmine]() gems.  Downloads the files required for [jasmine-jquery-rails]() and [jasmine-fixtures]().  Adds Jasmine to Guardfile and configures guard to run specs using jasmine-rails path.
