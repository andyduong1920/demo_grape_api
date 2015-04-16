Step 1:
	Add gem 'grape'

	bundle install

Step 2:
	Add

		config.paths.add 'app/api', glob: '**/*.rb'
    	config.autoload_paths += Dir["#{Rails.root}/app/api/*"]

    to config/application.rb

Step 3:
	Create folder app/api

	Create folder app/api/v1

			Create file app/api/v1/user_api.rd

	Create file root_v1.rb in app/api

Step 4:

	Change routes.rb

Ex: link for v1: /api/v1/users
