# Bubble-Sort-vs-Selection-Sort


Program Summary

The program is designed to read in an array of floating-point values (wind speeds), and sort the values using bubble sort and selection sort algorithms, calculating the time it took for each algorithm and displaying the number of comparisons and swaps each algorithm took. 
The second part of the program takes in the unsorted array data, I used the data in the data.h header file, and by using an array divided the data into five equally spaced partitions and displays it in a user-friendly format.

Issues Encountered & Solutions

First issue I encountered, was checking if the comparisons were correct, it was more time consuming than a real issue as I was checking with a small array and counting upwards, but thankfully I found another solution. For selections sort comparisons will equal n(n-1)/2, and for bubble sort comparisons are equal to (n-1) *(n-1), so although I’m not using the expressions in the actual code it was great to use to check if my sorting algorithms were counting comparisons correctly. I also made a function firstly that iterated the algorithm 10000 times to check the timer. It took a lot of playing around with as print functions were reproducing with it etc. To my dismay later I realised the data we would be using in the array was more than enough to put a timer on the sorting algorithms themselves (my fault for not going through the whole question first), either way I guess it is good to test that timings work. 
It also took me some time to realise that I needed to make a second unsorted array for my second algorithm as the data stayed sorted and the second algorithm had nothing to sort and therefore the output was coming back with 0 swaps. 
Figuring out how to use an array to partition the data was also a challenge, but with some research and a bit of reasoning I figured it out. I first used an if statement to get an understanding of the data and went from there.

Conclusion

This was a challenging assignment but a rewarding one, I have never used a header.h file before. This was great to learn, and I think will come in handy to keep my code tidy. I feel confident now using bubble sort & selection sort algorithms, even if they aren’t necessarily the fastest compared to other algorithms.
When I printed out the unsorted values into 5 partitions, I started with float values, I thought this was a more accurate representation of the data, but essentially, I changed it to the into integers as asked for. The values completely changed, which is obviously to do with the numbers being rounded, I thought this was worth noting here. (Photo Below)

 


Q9. When looking at the timing of both bubble sort and selection sort algorithms, it’s clear that selection sort is the faster of the two algorithms.



Pseudocode
1.	Create bubble sort and selection sort algorithm and place into a function that receives the raw floating-point data and sorts it.
2.	Use a header file to feed in data to arrays
3.	Add timer, swap & comparison counter to both sorting algorithms
4.	Print findings on both sorting algorithms to screen
5.	Create a function that receives a sorted array and prints to screen.
6.	Create a function that prints max and min wind speeds to screen 
7.	Use an array to partition the data in to 5 equal parts and converting data into integers 
8.	Display partitions on to screen using user-friendly format – use printf modifiers

