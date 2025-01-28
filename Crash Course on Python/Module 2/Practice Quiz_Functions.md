## 1. The function in the code below converts kilometers (km) to meters (m). In this exercise, you'll edit the code to:

		Complete the function so it returns the result of the conversion. 
		
		Call the function to convert the trip distance from kilometers to meters.
		
		Print a text string display the result of the conversion.
		
		NOTE: As you edit this code, do not change the indentation. If you do, it might return an error.
		
		# 1) Complete the code to return the result of the conversion
			def convert_distance(km):
			m = km * 1000  # exactly 1000 meters in 1 kilometer
			return m

		# Do not indent any of the following lines of code as they are
		# meant to be located outside of the function above
		
		
		my_trip_kilometers = 55
		
		
		# 2) Convert my_trip_kilometers to meters by calling the function above
		my_trip_meters = convert_distance(my_trip_kilometers)
		
		
		# 3) Fill in the blank to print the result of converting my_trip_kilometers
		print("The distance in meters is " + str(my_trip_meters))

## 2 Which of the following are good coding style habits?

	Adding comments
	
	Writing self-documenting code
	
## 3 What are the values passed into functions as input called?

	Parameters
	
## 4 Complete the first line of the “print_seconds” function so that it accepts three parameters: hours, minutes, and seconds. Remember, to define a function, you use the def keyword followed by the function name and parentheses. The function parameters go inside the parentheses in the function definition, and they represent the values that will be given to the function when it is called. Also remember that the print function is a built-in Python function that outputs its arguments to the console. You call a function by using its name followed by parentheses, with the arguments for the function inside the parentheses.

	def print_seconds(hours, minutes, seconds):
    print(hours*3600+minutes*60+seconds)

	print_seconds(1,2,3)
	#output will print to the screen
	
## 5 What is the purpose of the def keyword?

	Used to define a new function
