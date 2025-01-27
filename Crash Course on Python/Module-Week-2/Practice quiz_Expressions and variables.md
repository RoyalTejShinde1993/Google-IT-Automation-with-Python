
## 1 This code is supposed to display the equation 2 + 2 = 4 on the screen, but there is an error. Find the error in the code and fix it, so that the output displays the equation.

Note: Make sure the spaces between the components in your equation are identical to the spaces in the equation provided in the question. 

  print("2 + 2 = " + str(2 + 2))
  
    2 + 2 = 4
  
## 2 In this scenario, two friends are eating dinner at a restaurant. The bill comes in the amount of 47.28 dollars. The friends decide to split the bill evenly between them, after adding 15% tip for the service. Calculate the tip, the total amount to pay, and each friend's share, then output a message saying "Each person needs to pay: " followed by the resulting number.

	bill = 47.28  # Assign bill amount
	tip = bill * 0.15  # Multiply by 15% tip rate
	total = bill + tip  # Sum the bill and tip
	share = total / 2  # Divide total by number of friends (2)
    print("Each person needs to pay: " + str(round(share, 2)))  # Convert share to string and round to 2 decimal places

    Each person needs to pay: 27.19

## 3 This code is supposed to take two numbers, divide one by another so that the result is equal to 1, and display the result on the screen. Unfortunately, there is an error in the code. Find the error and fix it, so that the output is correct.
  
		numerator = 10
		denominator = 10       # Ensure denominator is not zero
		if denominator != 0:
			result = numerator / denominator
			print(result)
		else:
			print("Cannot divide by zero!")
	   
## 4 Combine the variables to display the sentence "How do you like Python so far?" 
  
     word1 = "How"
	 word2 = "do"
	 word3 = "you"
	 word4 = "like"
	 word5 = "Python"
	 word6 = "so"
	 word7 = "far?"
	 
	 print(word1 + " " + word2 + " " + word3 + " " + word4 + " " + word5 + " " + word6 + " " + word7)
