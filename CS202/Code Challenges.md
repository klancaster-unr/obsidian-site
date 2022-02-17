## [[Vectors]] and [[Iterators]]


1\. What happens when you run this code? Why are you getting this result?

```c++
std::vector<int> nums = { 1,2,3,4,5};  
auto it = nums.begin();  
while(it != nums.end()) {  
    std::cout << *it << std::endl;  
 it+= 2;  
}