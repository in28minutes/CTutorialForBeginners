# C Tutorial For Beginners

##Installing CDT In Eclipse
https://www3.ntu.edu.sg/home/ehchua/programming/howto/EclipseCpp_HowTo.html

##Online Editors
 - http://www.tutorialspoint.com/compile_c_online.php
 - https://www.google.co.in/search?q=c+online+compiler


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
