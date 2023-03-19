# BIG-BANG
Step 1: Copy the code

Step 2: Paste the code inside visual studio code or other IDE that support python

Step 3: Run the code

Step 4: Open the file that is created by the code under the name "output.json"

!!!There you go now you know when the BIG BANG will happen

    import json #import library

    output = [] #create a list

    for i in range(1, 101): #create a loop where the loop range is 1 to 100

        if i % 3 == 0 and i % 5 == 0: #check whether i is divisible by 3 and 5
            output.append("BIG BANG") #insert the word "BIG BANG" into the array if condition met

        elif i % 3 == 0: #check whether i is divisible by 3 
            output.append("BIG") #insert the word "BIG" into the array if condition met

        elif i % 5 == 0: #check whether i is divisible by 5
            output.append("BANG") #insert the word "BANG" into the array if condition met

        else: #if non of the condition above is met then the number i will be added into the array
            output.append(i)

    with open('output.json', 'w') as f: #to open/create a file

        json.dump(output, f) #use json.dump to dump/write all the value into the file created
