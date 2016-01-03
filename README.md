# C Tutorial For Beginners

* [Installing CDT In Eclipse](#installing-cdt-in-eclipse)
* [Online Editors](#online-editors)
* [All Code Examples](#all-code-examples)
  - [Hello World](#hello-world)
  - [First Variable](#first-variable)
  - [Two Variables](#two-variables)
  - [Sum of Two Variables](#sum-of-two-variables)
  - [Swap Program](#swap-program)
  - [Floating point variable](#floating-point-variable)
  - [Function](#function)
  - [IF ELSE](#if-else)
  - [Nested If Else](#nested-if-else)
  - [Switch Statement](#switch-statement)
  - [Need for an Array](#need-for-an-array-)
  - [Array Basics](#array-basics)
  - [For Loop Example](#for-loop-example)
  - [Do while Example](#do-while-example)
  - [Leap Year](#leap-year-c-program)
  - [Sum of first n numbers program](#sum-of-first-n-numbers-program)
  - [C Program Sum of First n even numbers](#c-program-sum-of-first-n-even-numbers)
  - [Divisors of a number](#divisors-of-a-number)
  - [Prime Number Program](#prime-number-program)
  - [Number of digits in a number](#number-of-digits-in-a-number)
  - [Sum of Digits Program](#sum-of-digits-program)
  - [Write to a file](#write-to-a-file)
  - [Read From File](#read-from-file)
* [About in28Minutes](#about-in28minutes)
  - [Our Beliefs](#our-beliefs)
  - [Our Approach](#our-approach)
  - [Find Us](#useful-links)

##Installing CDT In Eclipse
https://www3.ntu.edu.sg/home/ehchua/programming/howto/EclipseCpp_HowTo.html

##Online Editors
 - http://www.tutorialspoint.com/compile_c_online.php
 - https://www.google.co.in/search?q=c+online+compiler

#All Code Examples
#Hello World
```
#include <stdio.h>

int main() //pre-defined function
{
	printf("Hello World 123");
	return 0;
}
```

#Main is Main
```
#include <stdio.h>

int printSomething()
{
	printf("I will not be executed");
	return 0;
}

int main()
{
	printf("I'm a great guy");
	return 0;
}
```
#Print Something
```
#include <stdio.h>

void printSomething()
{
	printf("I will not be executed");
}

int main()
{
	printf("I'm a great guy");
	printSomething();
	return 0;
}

```
#First Variable
```
#include <stdio.h>

//Variable - value can change
//Assignment Operator

/////////
//  3  //
////////
//score - integer
int main()
{
	int score;//1854054454 
	//TYPE NAME;
	//d - integer
	printf("score : %d",score);
	return 0;
}

```
#Two Variables
```
#include <stdio.h>

//Assignment Operator

//////////////////
//  20  //
//////////////////
//score - integer
int main()
{
	int score1;//
	int score2;

	score1 = 5;
	score2 = 15;

	printf("score1 : %d \n",score1);

	printf("score2 : %d",score2);
	return 0;
}
```

#Sum of Two Variables
```
#include <stdio.h>

//Assignment Operator

//////////////////
//  20  //
//////////////////
//score - integer
int main()
{
	int score1;//
	int score2;
	int sum;

	score1 = 5;
	score2 = 15;

	sum = score1 + score2;

	printf("score1:%d score2:%d sum:%d",
			score1,score2,sum);
	return 0;
}
```

#Swap Program
```
#include <stdio.h>

//Assignment Operator

///////////   ///////////
//   10    //    //  10     //
//////////    //////////
// i               j

//score - integer
int main()
{
	int i=5;
	int j=10;
	int k;

	k = i;//k=5,i=5,j=10
	i=j;//k=5,i=10,j=10
	j=k;//k=5,i=10,j=5

	printf("i:%d j:%d",
			i,j);

	return 0;
}
```
#Floating point variable
```
#include <stdio.h>

int main()
{
	int i=1;
	int j=10;

	float avg;//1.5,2.5

	avg = (i+j)/2.0;

	printf("avg:%f",avg);
	//d - integer
	//f - float

}
```
#Character Example
```
#include <stdio.h>

int main()
{
	int i=1;
	int j=10;

	char ch = 67;//ASCII

	printf("ch:%c",ch);//A
	//d - integer
	//f - float
	//c - character

}
```

#Function
```
#include <stdio.h>

//REturnType NameofFuntion()
//{
// BODY;
//}
void welcome() //declaration
{
	printf("Hi From in28Minutes.com\n");
}

int main()
{
	welcome(); //calling or invocation
	welcome();
	welcome();
}
```
#IF ELSE
```
#include <stdio.h>

void welcome()
{
	printf("Welcome to in28minutes.com\n");
}

void subscribe() //declaration
{
	printf("Subscribe at in28Minutes.com\n");
}

int main()
{
	int like=0;
	welcome(); //calling or invocation

	if(like) // true if like has non zero
	{
		subscribe();
	}
	else
	{
		printf("Please tell us what we can do to improve");
	}
}
```
#Nested If Else
```
#include <stdio.h>

int main()
{
	int score=3;
	//1 - Single 2- Double
	//3 - Triple 4 - Boundary 6 - Sixer

	if(score==1)
	{
		printf("Single");
	}
	else if(score==2)
	{
		printf("Double");
	}
	else
	{
		printf("Something Else");
	}
}

```
#Switch Statement
```
#include <stdio.h>

int main()
{
	int score=6;
	//1 - Single 2- Double
	//3 - Triple 4 - Boundary 6 - Sixer

	switch(score)
	{
	case 1 :
		printf("Single");
		break;
	case 2 :
		printf("Double");
		break;
	default:
		printf("Something Else");
		break;
	case 4:
		printf("Boundary");
		break;
	}
}
```
#Need for an Array 
```
#include <stdio.h>

int main()
{
	int score1=6;
	int score2=15;
	int score3=145;
	int count = 0;

	if(score1>99)
		count = count + 1;

	if(score2>99)
		count = count + 1;

	if(score3>99)
		count = count + 1;

	printf("Number of Centuries %d",count);
}
```
#Array Basics
```
#include <stdio.h>
int main()
{
	int score1=106;
	int score2=15;
	int score3=145;
	int score4=23;

	int scores[10] = {106, 15, 145, 23};
				  // 0    1   2   3
	int scoresLength = 4;

	//How to read values?
	//printf("%d",scores[0]);
	//How to set values?
	scores[0] = 108;
	//How to find length of an array?
	//What is the default value?
	//printf("%d",scores[5]);//0
	//What if I try to bite more than I can Chew?
	printf("%d",scores[11]);//-1308602447

}
```
#For Loop Example
```
#include <stdio.h>
int main()
{

	int scores[] = {106, 15, 145, 23};
				  // 0    1   2   3
	int scoresLength = 4;

	for
	(
			int i = 0;//initialization
			i < scoresLength;//condition
			i++//increment
	)
	{
		printf(" %d ",scores[i]);
	}

}

```
#While Loop Example
```
#include <stdio.h>
int main()
{

	int scores[] = {106, 15, 145, 23, 235,235,235};
				  // 0    1   2   3
	int scoresLength = 7;

	int i = 0;//initialization

	while(i < scoresLength)//condition
	{//i:7
		printf(" %d ",scores[i]);
		i++;//increment
	}
	
	for(int i=0;i<scoresLength;i++)
	{
		printf(" %d ",scores[i]);
	}
}

```
#Do while Example
```
#include <stdio.h>
int main()
{

	int scores[] = {106, 15, 145, 23, 235,235,235};
				  // 0    1   2   3
	int scoresLength = 7;

	int i = 0;//initialization

	do
	{//i:7
		printf(" %d ",scores[i]);
		i++;//increment
	}
	while(i < scoresLength);//condition
}

```
#C Program : Print an Array
```
#include <stdio.h>

//returntype name(arguments)
void printArray(int array[],int length)
{
	for(int i=0;i<length;i++)
	{
		printf("%d ",array[i]);
	}
	printf("\n");
}

int main()
{
	int scoresTeam1[] = {10,101,25,47};
	int scoresLength = 4;
	int scoresTeam2[] = {10,100,5,7};

	printArray(scoresTeam1,scoresLength);
	printArray(scoresTeam2,scoresLength);
	return 0;
}
```

#Program - is number even?
```
#include <stdio.h>

//0 - false, anything non-zero - true (1,-1)
int isEven(int number)
{
	if(number%2==0)// 5%2==1 - comparision
		return 1;

	return 0;
}

//isEven
//2 - true
//3 - false
int main()
{
	printf("1:%d\n",isEven(1));
	printf("2:%d\n",isEven(2));
	return 0;
}



```
#Leap Year C Program
```
#include <stdio.h>

//0-false 1-true
int isLeapYear(int year)
{
	if(year%400==0)
		return 1;

	if(year%100==0)
		return 0;

	if(year%4==0)
		return 1;

	return 0;
}

//%4 = Leap YEar
//1900,2000,2100,2200,2300,2400

int main()
{
	printf("2000:%d\n",isLeapYear(2000));
	printf("1900:%d\n",isLeapYear(1900));
	printf("1904:%d\n",isLeapYear(1904));
	printf("1901:%d\n",isLeapYear(1901));

	return 0;
}

```
#Sum of first n numbers program
```
#include <stdio.h>

//0-false 1-true
int calculateSumUpto(int n)
{
	int result = 0;

	for(int i=1; i<=n; i++)
	{
		result = result + i;
	}

	return result;
	// 1 to n
	// result = result + index
}

// 5 =  1 to 5, 1 + 2 + ... + 5 = 15

int main()
{
	printf("upto 5:%d\n",calculateSumUpto(5));
	printf("upto 10:%d\n",calculateSumUpto(10));

	return 0;
}

```
#C Program Sum of First n even numbers
```
#include <stdio.h>

//0-false 1-true
int calculateSumEvenNumbersUpto(int n)
{
	int result = 0;

	for(int i=2; i<=n*2; i = i + 2) //1 to n 2,4,6,8,10
	{
		result = result + i; //1 to n  2 * 1 to 2 * n
	}

	return result;
	// 1 to n
	// result = result + index
}

// 5 =  1 to 5, 1 + 2 + ... + 5 = 15

int main()
{
	printf("upto 5:%d\n",calculateSumEvenNumbersUpto(5));
	printf("upto 10:%d\n",calculateSumEvenNumbersUpto(10));

	return 0;
}

```
#Divisors of a number
```
#include <stdio.h>

void printDivisors(int n)
{
	for(int i=2;i<n;i++){
		if(n%i ==0){
			printf("%d\n",i);
		}
	}
}

//12 - 2,3,4,6
int main()
{
	printDivisors(12);
	return 0;
}

```
#Prime Number Program
```
#include <stdio.h>

//0-Not prime
//1 - prime
// 12 (2, 3,4,...,11)
int isPrime(int n)
{
	for(int i=2;i<n;i++){
		if(n%i == 0){
			return 0;
		}
	}

	return 1;
}

//12 - 2,3,4,6
int main()
{
	printf("4 : %d\n",isPrime(4));
	printf("5 : %d\n",isPrime(5));
	return 0;
}

```
#Number of digits in a number
```
#include <stdio.h>

int numberOfDigits(int n) //345
{
	int temp = n;//0
	int count = 0;//3
	while(temp!=0)
	{
		count++;
		temp = temp/10;
	}
	return count;

}

//456 - 3
//24567 - 5

int main()
{
	printf("456: %d\n",numberOfDigits(456));
	printf("24567: %d\n",numberOfDigits(24567));
	return 0;
}

```
#Sum of Digits Program
```
#include <stdio.h>

//345
//34 - 5
//3  - 5 + 4
//0  - 5 + 4 + 3

int sumOfDigits(int n) //345
{
	int temp = n;//3
	int sum = 0;//0 + 5 + 4 + 3
	while(temp!=0)
	{
		sum = sum + temp % 10;
		temp = temp/10;
	}
	return sum;

}

//456 - 15
//24567 - 24

int main()
{
	printf("456: %d\n",sumOfDigits(456));
	printf("24567: %d\n",sumOfDigits(24567));
	return 0;
}

```
#Write to a file
```
#include <stdio.h>

struct Student
{
	char name[100];
	int marks;
	int year;
};

void writeStudentToFile(struct Student student)
{
	//Get a pointer to the opened file
	// w   1 = 1
	// r
	// a - 5 + 1 = 6
	FILE *fp = fopen("Student.dat","w");

	//Write to the file
	fprintf(fp,"%s %d %d\n",student.name,student.marks,student.year);

	//Close the file
	fclose(fp);
}

int main()
{
	struct Student student =
		{"in28Minutes",100,4};

	writeStudentToFile(student);
}

```
#Read From File
```
#include <stdio.h>

struct Student
{
	char name[100];
	int marks;
	int year;
};

struct Student readStudentFromFile()
{
	//Get a pointer to the opened file
	FILE *fp = fopen("Student.dat","r");
	struct Student student;

	//Read from the file
	fscanf(fp,"%s %d %d\n",student.name,&student.marks,&student.year);

	//Close the file
	fclose(fp);

	return student;
}

void printStudent(struct Student student)
{
	printf("%s %d %d\n",student.name,student.marks,student.year);
}

int main()
{
	struct Student student = readStudentFromFile();
	printStudent(student);
}

```

##About in28Minutes
- At in28Minutes, we ask ourselves one question everyday. How do we create more effective trainings?
- We use Problem-Solution based Step-By-Step Hands-on Approach With Practical, Real World Application Examples. 
- Our success on Udemy and Youtube (2 Million Views & 12K Subscribers) speaks volumes about the success of our approach.
- While our primary expertise is on Development, Design & Architecture Java & Related Frameworks (Spring, Struts, Hibernate) we are expanding into the front-end world (Bootstrap, JQuery, Angular JS). 

###Our Beliefs
- Best Course are interactive and fun.
- Foundations for building high quality applications are best laid down while learning.

###Our Approach
- Problem Solution based Step by Step Hands-on Learning
- Practical, Real World Application Examples.
- We use 80-20 Rule. We discuss 20% things used 80% of time in depth. We touch upon other things briefly equipping you with enough knowledge to find out more on your own. 
- We will be developing a demo application in the course, which could be reused in your projects, saving hours of your effort.
- All the code is available on Github, for most steps.

###Useful Links
- [Our Website](http://www.in28minutes.com)
- [Youtube Courses](https://www.youtube.com/user/rithustutorials/playlists)
- [Udemy Courses](https://www.udemy.com/user/in28minutes/)
- [Facebook](http://facebook.com/in28minutes)
- [Twitter](http://twitter.com/in28minutes)
- [Google Plus](https://plus.google.com/u/3/110861829188024231119)

###Other Courses
- [Spring Framework](https://www.udemy.com/spring-tutorial-for-beginners/)
- [Maven](http://www.in28minutes.com/p/maven-tutorial-for-beginners.html)
- [Eclipse](http://www.in28minutes.com/p/eclipse-java-video-tutorial.html)
- Java
  * [Java](https://www.youtube.com/watch?v=Y4ftqcYVh5I&list=PLE0D4634AE2DFA591&index=1)
  * [Java Collections](http://www.in28minutes.com/p/java-collections-framework-video.html)
  * [Java OOPS Concepts](https://www.udemy.com/learn-object-oriented-programming-in-java/) 
- [Design Patterns](http://www.in28minutes.com/p/design-patterns-tutorial.html)
- [JUnit](https://www.udemy.com/junit-tutorial-for-beginners-with-java-examples/)
- [C](https://www.udemy.com/c-tutorial-for-beginners-with-puzzles/)
- [C Puzzles](https://www.udemy.com/c-puzzles-for-beginners/)
- [Javascript](https://www.youtube.com/watch?v=6TZdD-FR6CY)
- [More Courses on Udemy](https://www.udemy.com/user/in28minutes/)
  * Java Servlets and JSP : Your first web application in 25 Steps
  * Learn Spring MVC in 25 Steps 
  * Learn Struts in 25 Steps 
  * Learn Hibernate in 25 Steps
  * 10 Steps to Professional Java Developer
- [Java Interview Guide](http://www.in28minutes.com/p/buy-our-java-interview-guide.html)
  * Core Java
  * Advanced Java
  * Spring, Spring MVC
  * Struts
  * Hibernate
  * Design Patterns
  * 400+ Questions
  * 23 Videos
  
  
