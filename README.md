Download Link: https://assignmentchef.com/product/solved-cs20a-quiz-1
<br>
<strong>True/False</strong>: Write out either True or False.

<ol>

 <li>If you do not define one the compiler will create an implicit constructor for your class.</li>

 <li>You can define more than one constructor for a class.</li>

 <li>When defining an instance of a class, member variables in that class are always initialized to known values.</li>

 <li>You can define more than one destructor for a class.</li>

 <li>Pointers in C++ are data types that store addresses.</li>

 <li>In C++ arrays are just pointers.</li>

 <li>Suppose you have an int pointer called ptr pointing to an integer array. C++ understands  *(ptr) + 2 to mean “move two integers down and retrieve that value”.</li>

</ol>

<strong>Multiple Choice: </strong>

<ol start="8">

 <li>Abstract Data Types consist of:

  <ul>

   <li>Data Structures.</li>

   <li></li>

   <li>An Interface.</li>

   <li>All mentioned.</li>

  </ul></li>

 <li>Which of these best describes the concept of ‘Encapsulation’?

  <ul>

   <li>Hides data and algorithms.</li>

   <li>Using single interface for general class of actions.</li>

   <li>Reduce Complexity.</li>

   <li>All mentioned.</li>

  </ul></li>

 <li>If a class’s data members are private, what can we do to access them from the class object?

  <ul>

   <li>Create public member functions to access those data members.</li>

   <li>Create private member functions to access those data members.</li>

   <li>Create protected member functions to access those data members.</li>

   <li>Private data members can never be accessed from outside the class.</li>

  </ul></li>

 <li>What is the difference between struct and class in C++?

  <ul>

   <li>All members of a structure are public and structures don’t have constructors and destructors.</li>

   <li>Members of a class are private by default and members of struct are public by default. When deriving a struct from a class/struct, default access-specifier for a base class/struct is public and when deriving a class, default access specifier is private.</li>

   <li>All members of a structure are public and structures don’t have virtual functions. d.) All mentioned.</li>

  </ul></li>

 <li>What is the output of the following program?</li>

</ol>

#include&lt;iostream&gt; using namespace std; class Point { public:

Point() { cout &lt;&lt; “Constructor called” &lt;&lt; endl; }

};

int main() {    Point t1, *t2;    return 0;

}




<ul>

 <li>Compiler Error.</li>

 <li>Constructor called</li>

</ul>

Constructor called c.) Constructor called

d.) Nothing will print.

<ol start="13">

 <li>You must include a class’s header file when.

  <ul>

   <li>Use the class as a parameter to a function.</li>

   <li>Use any of that class’s member functions.</li>

   <li>Declare a pointer or reference to that class.</li>

   <li>All mentioned.</li>

  </ul></li>

</ol>

<strong>Short Answer: </strong>

<ol start="14">

 <li>For this problem, you will be asked to write some code to accomplish a particular task given the code fragment below. Each task will depend on the tasks that came before it.  Your code must be syntactically correct.</li>

</ol>

int i1 = 100;  int i2 = -8;  int i3 = 15;

int *p1, **p2, ***p3;

<ul>

 <li>Set p1 to point to i1.</li>

 <li>Using p2 change the value of i1 to the value of i2.</li>

 <li>Using p3 make p1 point to i3</li>

 <li>What does the following code output? cout&lt;&lt; *&amp;*&amp;**&amp;*p2;</li>

</ul>

<ol start="15">

 <li>This following program is supposed print 30 20 10, but it does not. Find all the bugs and show fixed corrected version of the program. Note that cout&lt;&lt;”30 20 10”; is not a correct fix.</li>

</ol>

int main(){ int arr[3] = { 5, 10, 15 }; int* ptr = arr;




*ptr = 10;          // set arr[0] to 10 *ptr + 1 = 20;      // set arr[1] to 20 ptr += 2;

ptr[0] = 30;        // set arr[2] to 30

while (ptr &gt;= arr) { ptr–;

cout &lt;&lt; ‘ ‘ &lt;&lt; ptr;    // print values

}

cout &lt;&lt; endl;

}

<ol start="16">

 <li>Suppose you’re tasked with implementing a coin counter program for a digital piggy bank. The incomplete class declaration is as follows:</li>

</ol>

class CountingPiggy

{

public:

CountingPiggy ();      void addDollar();    // Add a dollar coin to the machine.  void addQuarter(); // Add a quarter to the machine. void addDime();     // Add a dime to the machine. void addNickel();    // Add a nickel to the machine. void addPenny();    // Add a penny to the machine.

void giveMeBills(); // Print what the user will get.

// See the example below.

private:

// TODO: Add private variables here.

};

The class’s usage may look like:

CountingPiggy  cp;  cp.addDollar();    // Currently $1.00. cp.addQuarter();    // Currently $1.25. for (int i = 0; i &lt; 10; i++) // Add 10 dimes, total becomes $2.25.  cp.addDime();   for (int i = 0; i &lt; 32; i++) // Add 32 pennies, total becomes $2.57.  cp.addPenny();   cp.giveMeBills(); // Produces the following output.

Output:

2 dollar bill(s)

2 quarter(s) 0 dime(s)

<ul>

 <li>nickel(s)</li>

 <li>penny(ies)</li>

</ul>

Implement all the member functions so that the machine works as intended.  Do not add or modify any of the public members.  You are free to add any private members as needed. It may be useful to recall that in C++ the modulus operator is % which gives you the remainder in a division operation.





