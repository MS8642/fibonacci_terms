# fibonacci_terms
Simple program that shows n number of Fibonacci terms.

terms_insert = int(input("State the number of terms"))

#The first terms to start the program.
t1 = 0
t2 = 1
nth = 0

if terms_insert == 1:   
    print("Fibonacci Number 1 = " + str(t2)+"")

else:
    terms_insert >1
    print ("Fibonacci Number 1 = " + str(t2)+"")
    for num in range (2, terms_insert+1):
        nth = t1 + t2
        print("Fibonacci Number "+ str(num) + " = " + str(nth) +"")
        t1 = t2 #replaces the old terms with new ones
        t2 = nth

# How it works: line 4 requests a user for a specific number of Fibonacci numbers 
# that the user wants to see.
# Next : the terms of 0 and 1 will be a starting point.
# Note: even though, 0 is strictly speaking not a part of
# Fibonacci sequence, it is required in this program 
# for the code to work correctly.
# Next: If the user just wants to see one term, then
# only t2 will be printed ( t2 = 1) 
# where 1 is the first term in the sequence.
# If the user wants to see more than 1 term,
# the first term (t2 = 1) will be printed
# then using "in range" function
# the code specifies that it wants to start 
# running the "in range" from number 2.
# It is done this way, since the first term was already printed.
# It will run up to the value inserted at "terms_insert" + 1
# since the "in range" function will stop before the last term.
# Line 18 shows the start of summing terms
# Which will subsequently be the number on the correct term position in Fibonacci sequence.
# For example: term number 2 is 1.
# Next: Line 20 saves the term t2 into t1 and stores the new nth term as t2 which 
# is used further in the code.
