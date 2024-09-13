#TPRG 2131-01
#Nadim Gutto
#Wk1 Exercise 2
#This code prompts the user for a string that matches one of the words in the list of
#allowed words given as an argument and returns the entered string.

def get_word(word_list): #Prompt the user for a word in the list of allowed words.
    
    while True:
    
        user_input = input("Please enter a word >") #Prompts the user to enter a word.
    
        if user_input in word_list: #Checks if the entered word is in the word list.
            print(user_input) #Prints the word the user inputs if it's in the word list.
            return user_input #Returns the valid word and exits the function.
        
        else:
            print("Wrong input, please try again >") #Lets the user know their input was not in the word list
                                             #and the loop prompts them to try again.

get_word(["dog", "cat", "horse"]) #Calls the funtion get_word.
