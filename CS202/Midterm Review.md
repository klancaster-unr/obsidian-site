## Midterm Exam Review 

This review is in the form of questions from past exams.

1. Assume that you are to create a program that models the relationship between a dog, its owner, and the fleas that live on the dog. Sketch the UML diagram that would correctly model the relationships between these entities. 

2. What is the difference between aggregation and composition? Provide an example situation where you would use each of these concepts.

3. You come across the following code in a code review: 
	
	```c++
	int getAge(){  
	 	int age;  
	 	cin >> age; 
	 	if(age < 20){ 
	     	 std::runtime_error("Please enter an age greater than 20");
	 	}  
	}
	```
	
    Is this an appropriate use of an exception? Why or why not? If not, how would you handle the issue of an age being input below the minimum required?

4. What is the difference, if any, between initializing a variable using () versus {}? For example, `int x(20.2)` vs `int x{20.2}`?

2. Create the following code snippets:
	1. You are given a class `Employee`. How would you declare a `std::vector`to hold a list of `Employee`objects using`std::unique_ptr`to insure that the `Employee`objects are correctly deleted when the vector is destroyed?
	2. Create an interface called `Runnable`that has the methods `run()`,`stop()`, and `int getStatus()`.
	3. Show how you would use an `range`for-loop to iterate over a vector that contains `Employee`pointers and print the each employee's name using the `getName`function.
	4. Assuming you had a cpp and h files for a class called `Boat` and the `main`function was held in a cpp file called `main_driver`, write the makefile needed to compile the application and generate an executable called `boatmanager`
	
6. Why is it a bad idea to make all your class attributes public?

7. What is the purpose of the `override` specifier in the following code snippet?
   ```void print(int number) override {}```

8. Create an abstract base class called `Instrument` with one virtual method called `play(int note)`. Create a class called `Trumpet` that publicly inherits from `Instrument`.` 





