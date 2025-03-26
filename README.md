# Password-Generator
This is the Random Password Generator Python coding project which has helped me practice my basic skills.  
I came up with a basic plan as my coding journey thus far is on Entry-level Python Programmer. My idea was that I wanted to generate a random password. I wanted it to be based on the user's preferences. I knew that there is a basic set of criteria that I must adhere to or fulfill in collecting the user's preferences.
- Length
- Should contain uppercase
- Should contain special characters
- Should contain digits
- Get all available characters
- Randomly pick the characters up to a specified length
- Ensure that I have at least one of each character type
- Ensure that the length is valid

The thought process behind the "import string" module comes from the fact that it will give me access to a list of all of the characters that are lowercase, uppercase, digits and special characters. This resulted in saving me time from having to manually write the characters myself. As you can see my naming of my function "def generate_password():" led my code into exactly what I want my definition of the code to be. I have adhered to the security password rule which requires the password to have above 4 character types, line 12. This allows each character type to be represented in my password. The .strip() function will prevent the password from having spaces in it. 

Notice that I have done the password characters as a list "required_characters = []" line 22 because I can keep appending values inside of it very easily and then later, I can take this list and convert it to a string, shuffle around the values inside of it and to make it more flexible. And there is a speed concern here, that it is faster to add items into a list rather than it is to keep creating a new string. 

I had to start by collecting all of the user preferences line 6, and make sure the length is valid line 7 - 9. And then get all of the characters that I can possible use. Generate all of the required characters that I needed to have in this password then get the remaining length after I have generated those. I proceeded to generating the password by randomly selecting characters from all of the valid ones that I can pick. Shuffle up whatever I have selected and convert it to a stringand return it back to the user. When returning something from the function it simply gives it back to whatever the function was called. In this case, password = generate_password() line 42. 
