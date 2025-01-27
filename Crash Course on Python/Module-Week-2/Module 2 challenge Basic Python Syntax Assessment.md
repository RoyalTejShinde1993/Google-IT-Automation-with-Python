## 1 Complete the code to output the statement, “Diego’s favorite food is lasagna”. Remember that precise syntax must be used to receive credit.

	name = "Diego"
	fav_food = "lasagna"
	print(name + "’s favorite food is " + fav_food) 
	
## 2 What's the value of this Python expression: "big" > "small"?

	False
	
## 3 In the following code, what would be the output?

	number = 4
	if number * 4 < 15:
		print(number / 4)
	elif number < 5:
		print(number + 3)
	else:
		print(number * 2 % 5)
		
		Answers:7
		
## 4 Consider the following scenario about using if-elif-else statements:Police patrol a specific stretch of dangerous highway and are very particular about speed limits.  The speed limit is 65 miles per hour. Cars going 85 miles per hour or more are given a “Reckless Driving” ticket. Cars going more than 65 miles per hour but less than 85 miles per hour are given a “Speeding” ticket.  Any cars going less than 65 are labeled “Safe” in the system.  

   Fill in the blanks in this function so it returns the proper ticket type or label.
   
   def speeding_ticket(speed):
    if speed:
        ticket = "Reckless Driving"
    elif speed:
        ticket = "Speeding"
    else:
        ticket = "Safe"
    return ticket


	print(speeding_ticket(87)) # Should print Reckless Driving
	print(speeding_ticket(66)) # Should print Speeding
	print(speeding_ticket(65)) # Should print Safe
	print(speeding_ticket(85)) # Should print Reckless Driving
	print(speeding_ticket(35)) # Should print Safe
	print(speeding_ticket(77)) # Should print Speeding

## 5 In the following code, what would be the output?

		test_num = 12
	if test_num > 15:
		print(test_num / 4)
	else:
		print(test_num + 3)

	Answers:15
	
## 6 Fill in the blanks to complete the function. The “identify_IP” function receives an “IP_address” as a string through the function’s parameters, then it should print a description of the IP address. Currently, the function should only support three IP addresses and return "unknown" for all other IPs.

	 def identify_IP(IP_address):
    if IP_address == "192.168.1.1":
        IP_description = "Network router"
    elif IP_address == "8.8.8.8" or IP_address == "8.8.4.4":
        IP_description = "Google DNS server"
    elif IP_address == "142.250.191.46":
        IP_description = "Google.com"
    else:
        IP_description = "unknown"
    return IP_address


	print(identify_IP("8.8.4.4")) # Should print 'Google DNS server'
	print(identify_IP("142.250.191.46")) # Should print 'Google.com'
	print(identify_IP("192.168.1.1")) # Should print 'Network router'
	print(identify_IP("8.8.8.8")) # Should print 'Google DNS server'
	print(identify_IP("10.10.10.10")) # Should print 'unknown'
	print(identify_IP("")) # Should Should print 'unknown'
	

