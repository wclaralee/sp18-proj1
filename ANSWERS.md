# Q0: Why is this error being thrown?
	Root routes to home#index, which tries to get a Pokemon model that dne.
# Q1: How are the random Pokemon appearing? What is the common factor between all the possible Pokemon that appear? *
		Seed file has pokemon without trainers.
# Question 2a: What does the following line do "<%= button_to "Throw a Pokeball!", capture_path(id: @pokemon), :class => "button medium", :method => :patch %>"? Be specific about what "capture_path(id: @pokemon)" is doing. If you're having trouble, look at the Help section in the README.
	Capture_path(id: @pokemon) routes to /pokemon/id/capture, letting us create a button that calls the capture method for the given pokemon id, setting its trainer to the current logged in trainer.
# Question 3: What would you name your own Pokemon?
	Daisy the Jindo
# Question 4: What did you pass into the redirect_to? If it is a path, what did that path need? If it is not a path, why is it okay not to have a path here?
redirect_to trainer_path(current_trainer) Path needs the id of the current trainer to redirect to the profile page.
# Question 5: Explain how putting this line "flash[:error] = @pokemon.errors.full_messages.to_sentence" shows error messages on your form.
	The errors that a created when youre making new pokemon are stored in @pokemon.errors.full_messages.to_sentence. The flash line lets us display our form again after an error, but when we do that, the error message will show. The :error key lets us use the built in components to display errors. 
	
# Give us feedback on the project and decal below!
	Lots of fun, wish school didn't get in the way of full focus to this haha. 
# Extra credit: Link your Heroku deployed app
