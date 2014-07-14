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
  - Adds [haml](https://github.com/haml/haml) and [haml-rails](https://github.com/indirect/haml-rails) gems.  Also replaces default application layout file with a haml version.
- `--rspec`
  - Adds the [rspec-rails](https://github.com/rspec/rspec-rails),[factory_girl_rails](https://github.com/thoughtbot/factory_girl_rails), [faker](https://github.com/stympy/faker), [shoulda-matchers](https://github.com/thoughtbot/shoulda-matchers), [guard-rspec](https://github.com/guard/guard-rspec), and [simplecov](https://github.com/colszowka/simplecov) gems.  Installs RSpec into application.  Alters .rspec file to provide pretty output and require correct config file.  Adds common directories for RSpec tests.  Creates a binstub for RSpec.  Adds RSpec entry to Guardfile.  Adds RSpec to simplecov reports.
- `--cucumber`
  - Adds the [cucumber-rails](https://github.com/cucumber/cucumber-rails), [selenium-webdriver](https://github.com/vertis/selenium-webdriver), [database_cleaner](https://github.com/DatabaseCleaner/database_cleaner), [launchy](https://github.com/copiousfreetime/launchy), and [guard-cucumber](https://github.com/guard/guard-cucumber) gems.  Installs Cucumber into application.  Creates binstub for Cucumber. Configures the DatabaseCleaner.  Adds Cucumber entry to Guardfile.  Adds Cucumber to simplecov reports. 
- `--jasmine`
  - Adds the [jasmine-rails](https://github.com/searls/jasmine-rails), [jasmine-jquery-rails](https://github.com/travisjeffery/jasmine-jquery-rails), and [guard-jasmine](https://github.com/guard/guard-jasmine) gems.  Downloads the files required for [jasmine-jquery-rails](https://github.com/travisjeffery/jasmine-jquery-rails/tree/master/vendor/assets/javascripts) and [jasmine-fixtures](https://github.com/searls/jasmine-fixture).  Adds Jasmine to Guardfile and configures guard to run specs using jasmine-rails path.
- `--unicorn`
  - Adds the [unicorn](https://github.com/defunkt/unicorn) gem.  Creates *Procfile* and *Procfile.dev* files.  Creates *unicorn.rb* configuration files.  Redirects unicorn logging to stdout.
- `--bootstrap`
  - Adds the [bootstrap-sass](https://github.com/anjlab/bootstrap-rails) and [autoprefixer-rails](https://github.com/ai/autoprefixer-rails) gems.  Replaces *application.css* file  with *application.css.scss* file and adds bootstrap to it.  Adds *bootstrap-custom.css.scss* file for overrides to bootstrap default styles.  Adds bootstrap to *application.js* file.
