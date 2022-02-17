## Solution using Simple Array

This is one solution to loading a simple array with words from a file. It is certainly not the only solution.
How would you improve the solution?

```c++
void readWordsIntoArray() {  
 std::string inputFile = "myfile.txt";  
 std::ifstream dataFile(inputFile);  
 if(dataFile.fail()){  
 	std::cout << "Could not find file" << std::endl;  
 	exit(1);  
 } 
 std::string word;  
 std::string array[50];  
 int index = 0;  
 while(dataFile >> word && index < 49){  
 	array[index++] = word;  
 	std::cout << index << std::endl;  
 } 
 for(std::string s : array){  
	 std::cout << s << std::endl;  
 } 
 dataFile.close();  
}
```

### Some things to notice...
- Line 15 uses an [[enhanced for loop]]

