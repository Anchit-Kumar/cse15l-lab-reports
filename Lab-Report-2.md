# Lab Report 2

## Part 1 - String Server 
![Image of my StringServer.java code](https://anchit-kumar.github.io/cse15l-lab-reports/Screenshot%202023-01-30%20at%201.30.58%20AM.png)
  
![add-message screenshot 1](https://anchit-kumar.github.io/cse15l-lab-reports/Screenshot%202023-01-30%20at%201.38.09%20AM.png)

Here, the main method of the StringServer class is called first which in turn calls the Handler class. \
In the handler class, the handleRequest method is called with the argument passed as http://localhost:3241/add-message?s=Hello \
The handleRequest method then implements its 'else if' part which changes the value of the variable storedString by adding the \
part of the query after "?s=" to the string variable along with a new character and displays the string as it is currently on the \
webpage.

![add-message screenshot 2](https://anchit-kumar.github.io/cse15l-lab-reports/Screenshot%202023-01-30%20at%201.38.53%20AM.png)
Similarly, in this screenshot the main method of the StringServer class is called again which in turn calls the Handler class. \
In the handler class, the handleRequest method is called with the argument passed as http://localhost:3241/add-message?s=Welcome%20to%20my%20web%20server! \
The handleRequest method then implements its 'else if' part which changes the value of the variable storedString by adding the \
part of the query after "?s=" to the string variable along with a new character and displays the string as it is currently on the \
webpage. This displays both the strings on different lines as can be seen above.
  

## Part 2 

* A failure-inducing input for reversedInPlace was the array {2, 3, 5, 4} which it was unable to reverse in place. \
` 
  @Test 
	public void testReverseInPlace() {

    int[] input2 = {2, 3, 5, 4};
    ArrayExamples.reverseInPlace(input2);
    assertArrayEquals(new int[]{4, 5, 3, 2}, input2);
    
	}
`
  
* An input that did not induce a failure was an array with just one element { 3 } \
`
	@Test 
	public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}
`
* The symptom as the output of running the tests is as can be seen in the image below: \
![Image of running both the tests](https://anchit-kumar.github.io/cse15l-lab-reports/Screenshot%202023-01-30%20at%202.10.33%20AM.png)
  
* The method reverseInPlace was originally:
`
   static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
 `
 
 After the fix, the method reverseInPlace became:
 `
   static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) {
      int orgElmnt = arr[i];
      arr[i] = arr[arr.length - i - 1];
      arr[arr.length - i - 1] = orgElmnt;
    }
  }
 `
   
The bug in the original method was basically that it'd switch the elements up to halfway in the array with the correponding \
element from the end of the array but not the other way around. So when the for loop would go past the halfway point of the array, \
it would just replace the element with the element at the corresponding element at the beginning of the array but this would just replace \
the element with itself since the elements in the beginning have already been replaced. 
  
To solve this issue, I changed the for loop to only go up to the halfway point in the array and replace both elements at the same time. \
This works with both even and odd arrays since the integer division rounds down so for a four element array it would switch elements 1 and 4 \
and then 2 and 3 and stop. For an odd array of length 5, it would switch elements 1 and 5, 2 and 4 and then stop. Since element 3 is in the middle \
anyways, it doesn't need to switch. 
  

## Part 3
Something I learned in week 2 and week 3 lab that I didn't know of before was how to code and host a web server. I kind of knew how web servers and urls \
worked but really thinking of everything from the fundamentals and deploying my own web server really solidified my understanding. I now really understand \
the different parts of an url and what role they play in a web query and also ports used to be really confusing to me before. 
