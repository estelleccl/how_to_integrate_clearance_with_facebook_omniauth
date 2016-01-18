#Errors and Solution for Clearance gem

1. <b><i>ActiveRecord::StatementInvalid in SessionsController#create_from_omniauth Could not find table 'authentications' authentication = Authentication.find_by_provider_and_uid(auth_hash["provider"], auth_hash["uid"]) || Authentication.create_with_omniauth(auth_hash) </i></b>


	Solution:
		```create authentication table with uid,token and provider column```

2. <b><i>NoMethodError in SessionsController#create_from_omniauth undefined method `friendly_name=' for #<User:></i></b>
	
	Solution:
		``` add ``` friendly_name ``` column to users table ```

3. <b><i>NoMethodError in SessionsController#create_from_omniauth undefined method `picture =' for #<User:></i></b>

	Solution:
		``` add ``` picture ``` column to users table ```

4. <b><i>NoMethodError in SessionsController#create_from_omniauth undefined method `friendly_name =' for #<User:></i></b>

	Solution:
		``` add ``` friendly_name ``` column to users table ```
5. <b><i>NoMethodError in SessionsController#create_from_omniauth undefined method `last_name =' for #<User:></i></b>

	Solution:
		``` add ``` last_name ``` column to users table ```
6. <b><i>ActiveModel::MissingAttributeError in SessionsController#create_from_omniauth can't write unknown attribute `user_id</i></b>

	Solution:
		``` add ``` user_id ``` column to authentications table ```
