


                                                               #For loop

->Generally, it is very efficient to use this loop when the number of repetition is known is advanced.
->For statement is sometimes called as counted loop
->Syntax:	1		2		4
	for([initialization],[condition],[increment/ decrement]){
		3
[Statement body];
}
->Initialization: commonly an assignment to the control variable.
->Test-condition: This determines when the loop terminates.
->Increment/ Decrement: value of the control variable increases or decreases.
->Statement body: This can be multiple, single or even no statement at all.

Initialization—->Test condition—----> Body of loop—----> Increment/ Decrement
		—->False—--------------------------------------->

NOTE: Square brackets[] shows the optional part which may not be a part of syntax. Also, there must always be a semicolon “;” to specify the initialization condition and increment/ decrement section.

—------------------------------------------------------------------------------------------------------------------------
#WAP TO DISPLAY FROM 1 TO 10;

#include<stdio.h>
Int main()
{
	Int num;
	for(num=1;num<=10;num++)
{
	printf(“%d\n”,num);
}

Return 0;
}
—------------------------------------------------------------------------------------------------------------------------







—------------------------------------------------------------------------------------------------------------------------

#WAP TO DISPLAY FIRST 20 whole numbers AND FIRST 20 NATURAL NUMBERS

#include<stdio.h>
Int main()
{
	Int wNum, nNum;

	for(nNum=1; nNum<=20; nNum++)
{
	printf(“NATURAL”);
	printf(“%d\n”,nNum);                                                       
}

for(wNum=0; wNum<=19; wNum++)
{
	printf(“WHOLE”);
	printf(“%d\n”,wNum);
}

Return 0;
}
—------------------------------------------------------------------------------------------------------------------------

#WAP TO DISPLAY THE EVEN NUMBERS IN THE FIRST 50 NATURAL NUMBERS;

#include<stdio.h>
void main()
{
	int ev;
	for(ev=2;ev<=50;ev+=2)
	{
		printf("%d\t",ev);
	}

}
—------------------------------------------------------------------------------------------------------------------------





#WAP TO CHECK PRIME OR NOT;
#include<stdio.h>
void main()
{
	int prime,i,count=0;
	printf("Enter a number:");
	scanf("%d",&prime);
	
	for(i=1;i<=prime;i++)
	{
		if(prime%i==0)
		{
			count++;
		}
	}
	if(count==2)
	{
		printf("PRIME");
	}
	else
	{
		printf("NOT PRIME");
	}

}
—------------------------------------------------------------------------------------------------------------------------

#WAP TO FIND FACTORIAL

#include<stdio.h>
int main()
{
	int num2=1,num,order=1;
	printf("Enter a number:");
	scanf("%d",&num);
	
	for(order=1;order<=num;order++)
	{
		num2=order*num2;
	}
	printf("%d is the factorial.",num2);
	return 0;
}
—------------------------------------------------------------------------------------------------------------------------
#COMMA OPERATOR IN FOR LOOP
-> Comma operator (,) is used to permit two different operators in a context which were generally done by using one expression.
-> For example, for (Expression-A1, Expression-A2; Expression_B; Expression_C) Where Expression-A1 and Expression-A2 are two expressions that would be used within the for loop.
-> Another example; for (Expression_A1, Expression_A2; Expression_B; Expression_Of Expression(2) where Expression_C1, Expression_C2 are separated by comma operator and can be used to increase or decrease the value of the Expression_A1, Expression_A2 respectively.

#NESTED LOOP
-> A single or multiple loop statement within a loop is called a nested loop.
-> Similar types of loop can be nested or different types of loop can also be nested.
-> First, the innermost loop completes its total iterations then the loop outside it gets the chance to iterate.
-> In simple terms, a loop may act as a body or part of the body of another loop.
-> Syntax (nested for loop)
	for([initialization];[condition];[increment/ decrement]){
	//[statement];
	for([initialization];[condition];[increment/ decrement])
{
		[statement body];
}
//[Statement]
}
-> Similarly, while do while can also have a nested version of the structure.

—----------------------------FIGURE IN COPY—-----------------------------

			INITIALIZATION
FALSE								TRUE
END OF LOOP					INITIALIZATION
								TEST CONDITION
						FALSE				TRUE
						END OF LOOP		BODY OF LOOP
									INCREMENT/ DECREMENT
									CONTINUE THE LOOP
			CONTINUE THE LOOP
			INCREMENT/ DECREMENT





#WAP TO DISPLAY PRIME NUMBERS IN THE FIRST 50 NATURAL NUMBERS.
#include<stdio.h>
void main()
{
	int num,count,num2;
	for(num=1;num<=50;num++)
	{
		count=0;
		for(num2=1;num2<=num;num2++)
		{
			if(num%num2==0)
			{
				count++;
			}
			
		}
		if(count==2)
		{
			printf("%d\t",num);
		}
		else
		{
			printf("");
		}
	}
}



#WAP TO DISPLAY PATTERNS:
		#include<stdio.h>
void main()
{
	int i,j,k;
	for(i=1;i<=4;i++)
	{
		for(j=1;j<=4;j++)
		{
			printf("*");
		}
		printf("\n");
	}
}


#WAP TO DISPLAY THE PATTERN
*
**
***
****
*****

#include<stdio.h>
void main()
{
	int i,j,k;
	for(i=1;i<=5;i++)
	{
		for(j=1;j<=i;j++)
		{
			printf("* ");
		}
		printf("\n");
	}
}




#WAP TO PRINT THE PATTERN
*****
****
***
**
*
#include<stdio.h>
void main()
{
	int i,j,k;
	for(i=1;i<=5;i++)
	{
		for(j=5;j>=i;j--)
		{
			printf("*");
		}
		printf("\n");
	}
}
#WAP TO DISPLAY
******
  ****
   ***
    **

#include<stdio.h>
void main()
{
	int i,j,k;
	for(i=1;i<=5;i++)
	{
		for(j=5;j>=i;j--)
		{
			printf("*");
		}
		printf("\n");
	}
}


#WAP TO DISPLAY
  *
 ***
*****
#include<stdio.h>
void main()
{
	int i,j,k;
	for(i=1;i<=3;i++)
	{
		for(k=2;k>=i;k--)
		{
			printf(" ");
		}
		for(j=1;j<=2*i-1;j++)
		{
			printf("*");
		}
		printf("\n");
	}
}


#WAP TO DISPLAY
*****
 ***
  *
#include<stdio.h>
void main()
{
	int i,j,k;
	for(i=1;i<=3;i++)
	{
		for(k=1;k<=i;k++)
		{
			printf(" ");
		}
		for(j=5;j>=2*i-1;j--)
		{
			printf("*");
		}
		printf("\n");
	}
}


#WAP TO DISPLAY
  *
 ***
*****
 ***
  *
#include<stdio.h>
void main()
{
	int i,j,k;
	for(i=1;i<=3;i++)
	{
		for(k=3;k>=i;k--)
		{
			printf(" ");
		}
		for(j=1;j<=2*i-1;j++)
		{
			printf("*");
		}
		printf("\n");
	}

	for(i=1;i<=2;i++)
	{
		for(k=0;k<=i;k++)
		{
			printf(" ");
		}
		for(j=3;j>=2*i-1;j--)
		{
			printf("*");
		}
		printf("\n");
	}
}


#JUMPING STATEMENTS
-> It is an unconditional branching technique known as jump statements.
-> There are four kinds of jump statements in C programming.
Break Statement
Continue statement
Goto Statement 
Return Statement
-> The goto and return statements can be used anywhere in the program whereas, break and continue can be used in consideration to any loop statements.

#BREAK STATEMENTS
-> It is used in loops and switch cases.
-> In loop structure, a break statement is used to immediately terminate a loop without considering the loop termination condition and then pass the control to the next instruction 
while (condition 1){
Statement;
if(condition 2)
Break;
Statement;
}
Do{
Statement;
if(condition 1)
break;
}while(condition 1);
Statement
};
#WAP TO DISPLAY BREAK IN NESTED 
#include<stdio.h>
void main()
{
	int i,j;
	for(i=1;i<=3;i++)
	{
		printf("OUTER LOOP NUMBER[%d]\n",i);
		for(j=1;j<=3;j++)
		{
			if(i==2)
			printf("\t Break occurs in iteration [%d]",i);
			break;
		}
		printf("\n");
	}

}

#CONTINUE STATEMENTS

-> It is used to discontinue any remaining part of the current iteration in a loop.
-> This is simply used to Jump to the start of the loop to continue to the next iteration while discarding any remaining statement of the current iteration-it possesses through a current station of the loop without letting it execute body statements completely to approach for next status of the loop.

-While(condition 1){
	Statement;
	if(condition 2)
		-continue ;
	Statement;
}













#WAP to display the continue statement in a nested for loop.
#include<stdio.h>
void main()
{
	int i,j;
	for(j=1;j<11;j++)
	{
		printf("Outer Loop Number[%d]\n",j);
		for(i=1;i<11;i++)
		{
			if(i==2)
			{
				continue;
			}
			printf("\n\t Inner Loop Number [%d]",i);
		}
		printf("\n");
	}
}
 


#GOTO STATEMENTS
-> This statement is used to change the control flow of the program without much relying on a condition-unconditionally transfers the control to the other specific parts of the program.
-> A label with a double colon(:) is used to represent a single/ group of statements and a goto label statement is used to pass the control to the statement immediately following that label.
-> General form and Example:
	Goto Label;
	========
	Label:
		Statement;
	========
-> Here, in this example, when goto label is encountered than the statement after goto is skipped to unconditionally jump to statement after the “Label”
->The use of goto is considered to make a program unreliable; however, it is useful in special situations such as branching around statements, by passing the remaining part of a loop or even jumping out of a loop regardless of the termination condition of the loop.






#WAP TO DISPLAY GOTO
#include<stdio.h>
void main()
{
	int i,j;
	printf("Enter an integer number:\n");
	scanf("%d",&j);
	if(j<11)
	{
		goto statement1;
	}
	printf("Statement before the label, because you entered number greater than 10\n");
	goto jump_over;
	statement1:
		printf("Statement within the label");
	jump_over:
		return 0;
}


#RETURN STATEMENTS
-> Generally, it is used in the function to return to the point from where a call to the function was made.
-> It may or may not return a value from a function.
-> A function declared with the return type can only use a return statement with an expression -expression is used to return value.
-> A function declared without any return type is a void type function which requires no return statement.
-> Generally form: return expression.
-> EXAMPLE:
Int add(int x, int y){
	return(x+y);
} 

PRACTISE:
Qn1.WAP TO CHECK WHETHER THE YEAR ENTERED BY THE USER IS LEAP YEAR OR NOT
#include<stdio.h>
void main()
{
	int year;
	printf("Enter a year:");
	scanf("%d",&year);
	
	if(year%4==0)
	{
		printf("Leap year");
	}
	else
	{
		printf("Not leap year");
	}
}


Qn2. WAP TO DISPLAY SUM OF FOLLOWING SERIES UP TO N TERMS SUM=x-x2+x3-x4…..
#include<stdio.h>
#include<math.h>
void main()
{
	int i,num,count,sum1=0,sum2=0,total=0,total1=0,total2=0;
	printf("ENTER THE COUNT:");
	scanf("%d",&count);
	printf("ENTER THE NUMBER:");
	scanf("%d",&num);
	for(i=1;i<=count;i++)
	{
		if(i%2==0)
		{
			sum1=-pow(num,i);
			total1=total1+sum1;
		}
		else
		{
			sum2=pow(num,i);
			total=total1+sum2;			
		}
		total=total1+total2;
		
	}
	printf("SUM=%d \t %d\t %d",total1,total2,total);
}



Qn3. WAP TO CALCULATE SUM OF HARMONIC MEAN (1+½+⅓+...1/n) for given value of n

Qn4.	1
	23
	345
	4567
	56789

Qn5.   1
	22
	333
	4444
	55555
	666666

Qn6.WAP TO READ A NUMBER FROM USER AND SHOW ITS MULTIPLICATION TABLE FROM 1-20

Qn7.WAP TO CONVERT THE RANGE(0-50).c into .f

Qn8.WAP TO PRINT A SEQUENCE 1.5.9.13—up to 10th term

Qn9.WAP TO DISPLAY SUM OF EVEN NUMBERS UP TO n terms



#UNIT 6: Arrays and Strings
-> An array is an identifier that is a collection of elements of the same data type stored in a contiguous memory location.
-> Every data in an array is represented by the same name but differs in context with the position in the chain of memory.
-> Each data in an array is called an element of the array where each of these elements reside in a unique memory location in context with one another for a particular array.
-> In simple words, each item or element of an array shares the variable name but is uniquely identified by the index number.
-> Therefore to refer to any element of an array, an array in arms with the index number between square brackets is used.
-> For e.g; for an integer type array of size 5, we can declare an array as
	Int mem[5]={12,35,85,96,78}
	Int- data type of array
	Mem- array name which is mem in this example
[5]- Size of the array which is 5 in this example
-> Here, in this example, an integer type array with name mem is declared which can hold 5 different integers that can be accused of using its index.
 -> In an array, we can store multiple similar types of data with just a single identifier instead of using multiple variables to store those data items. 
-> Arrays are very efficient to store when related data items, such as roll number, marks obtained by students etc.
->An array can be single dimensional or multidimensional.
-> rather than during the run time, memory for an array element is allocated.
-> The size of the memory has to be guessed in advance which cannot be increased or decreased during run time once the memory has been allocated during allocation.

#TYPES OF ARRAYS
-> There are two major categories of array:
Based on numerical type:
-> Numeric and Non-numeric types.
Based on dimension
-> Single dimensional (1-Dimension) and Multi-Dimensional (N-Dimension)

# NON-NUMERAL ARRAY
-> Also known as Arrays of character or non-numeric array or character string or string.
-> Always represent symbols.
-> String related manipulation or operation requires string.h header file.
-> Example of data type: char

-> Based on dimension:
	-> Dimension refers to the whole subscript part of an array.
	-> An array may have a single subscript([size]) for one dimension or two subscripts ([size] [size]) for two dimensions.
-> Single dimensional( 1-Dimensional array):
-> An array with a single subscript member is referred to as an array or vector.

-> Multi dimensional (N-Dimensional array):
-> An array with multiple (more than one) subscript members is called a multiple dimensional array or matrix. 

#SINGLE DIMENSION ARRAY
-> Basically, a list of items with the same type can  be continuously stored in a variable using a single index that shows the position of an element within the array, such a type of variable is called a one-dimensional array or single subscripted variable.
-> In C, one-dimensional array AI can be represented as;
	A[0],a[1],a[2],a[n].
-> NOTE: Index always starts from 0.

#DECLARATION OF ONE-DIMENSIONAL ARRAY
-> An array of one dimension can be declared as:
	data -type array-name[size/subscript];
-> Different examples are:
	Int n[5]; // n is an array of 5 integers. This array stores 5 integers from n[0].....n[4]
Float a[7]; //  a is an array of 7 floating point values.
Long Long int x[20];// X is the long long type integer array of size 20.
Char h[20];// h is the char array of size 20
-> Note: When declaring an array the name of array is followed by square brackets([]) which contains subscript that shows the total number of member an array can hold i.e. shows the size of an array when an array is used for data operation, the array is followed by the subscript that contains an index which is an integer number that shows the exact location of an item or member of the array.
-> Also, there must not be a space between an array and the square bracket that follows it. The size of the array must be a constant integer number. Arrays act as a block of memory, therefore, the compiler must be able to examine and allocate the proper amount of memory to the array, during the compilation phase.

#INITIALIZATION OF ONE DIMENSIONAL ARRAY
-> Initialization while declaring:
	Data_type array_name[N] = {element1,.....element N};
-> Initialization by explicitly admitting# the dimension:-
	Int n[4]= {1,2,4,7},// n is an array of 4 integers
-> Initialization without explicitly writing the dimension:
Int n[ ]= {1,2,4,7};
-> Individual initialization: It is done after the declaration part whatever in the program but before the use of the element for processing. Example:
n[0]=1;
n[1]=2;
  
            n[2]=4;
n[3]=7;

#READING, ACCESSING AND DISPLAYING THE ELEMENTS IN 1-D ARRAY

-> For reading an element from the user for the numeric type array, formatted input function scanf can be used as;		scanf(“% characterConversion”, &arrayName[index]);
-> For reading all the elements of an entire array, the above scanf statement can be used in a loop where the loop iterates from 0 to ((size of the array)-1).
-> For accessing an element of an array, direct array name with the specific index can be used as;	arrayName[index];
-> For displaying an element of the numeric type array, formatted output function printf can be used as;	printf(“% conversionCharacter”, arrayName[index]);
-> For displaying all the elements of an entire array, the above printf statement can be used in a loop where the loop iterates from 0 to ((sizeOfAnArray)-1).

#ONE_DIMENSIONAL ARRAY: EXAMPLE




#WAP TO INITIALIZE AN INTEGER TYPE ARRAY WHILE DECLARING, WHERE ARRAY IS OF SIZE 8. ALSO, DISPLAY ALL THE ELEMENTS OF THE ARRAY.
 #include<stdio.h>
void main()
{
	int i,num[8]={2,3,4,2,3,5,4,6};
	printf("DISPLAYING:\n");
	for(i=0;i<8;i++)
	{
		printf("\nnum[%d]=%d",i,num[i]);
	}
}


#WAP TO FIND THE SUM OF qn1

#include<stdio.h>

int main(){
	int i= 0,sum = 0;
	int num[8] = {1,2,3,4,5,6,7,8};
	while (i<=7){
		sum = num[i] + sum;
		i += 1;
	}
	printf("Sum = %d", sum);
	return 0;
}

#WAP TO USER DEFINED
#include<stdio.h>
void main()
{
	int i,num[8],sum=0;
	printf("DISPLAYING:\n");
	for(i=0;i<8;i++)
	{
		printf("\nnum[%d]=",i);
		scanf("%d",&num[i]);
		sum+=num[i];
	}
		for(i=0;i<8;i++)
	{
		printf("\nnum[%d]=%d",i,num[i]);
	}
	
	printf("\nSum is %d",sum);
}



#WAP to get and display 10 integers and 10 floating point values using an array.
#include<stdio.h>
int main(){
	int i,num1[10];
	float num2[10];
	
	
	for (i=0;i<10;i++){
		printf("\n num1[%d]=",i);
		scanf("%d",&num1[i]);
	}
	printf("\n integer values are:\n");
	for(i=0;i<10;i++)
	{
		printf("\nnum[%d]=%d",i,num1[i]);
	}

	printf ("\n"); 

		for (i=0;i<10;i++){
		printf("\n num2[%d]=",i);
		scanf("%f",&num2[i]);
	}
	printf("\n floating values are:");
	for(i=0;i<10;i++)
	{
		printf("\nnum[%d]=%.2f",i,num2[i]);
	}

	return 0;
}




#WAP TO REVERSE ELEMENTS IN C
#include<stdio.h>
void main()
{
	int i,num[5]={1,2,3,4,5};
	for(i=4;i>=0;i--)
	{
		printf("%d \t",num[i]);
	}
	
}




#WAP TO DISPLAY MARKS OF 5 STUDENTS USER DEFINED
#include<stdio.h>
void main()
{
	float marks[3],sub[3];
	int i;
		printf("Enter the marks:\n");
	for(i=0;i<5;i++)
	{
		printf("Subject %d=",i+1);
		Scanf("%f",&sub[i]);
	}
	for(i=0;i<5;i++)
	{
		printf("\nSubject %d= %.2f",i+1,sub[i]);
	}
	
}




#WAP TO DISPLAY PERCENTAGE FROM MARKS OF 5 SUBJECTS
#include<stdio.h>
void main()
{
	float per,mark=0,sub[3];
	int i;
		printf("Enter the marks:\n");
	for(i=0;i<5;i++)
	{
		printf("Subject %d=",i+1);
		scanf("%f",&sub[i]);
	}
	for(i=0;i<5;i++)
	{
		printf("\nSubject %d= %.2f",i+1,sub[i]);
	}
	printf("\nThe percentage is\n");
	for(i=0;i<5;i++)
	{
		mark+=sub[i];
	}
	per=(mark/500.0)*100.0;
	printf("PERCENTAGE = %.2f",per);
}

#WAP TO INITIALIZE AN ARRAY OF SIZE 5 and DISPLAY THE SMALLEST ELEMENT IN THE ARRAY

#include<stdio.h>
void main()
{
	int num[5],i,j,check;
	printf("Enter the numbers:");
	for(i=0;i<5;i++)
	{
		printf("num[%d]=",i);
		scanf("%d",&num[i]);
	}
	check=num[0];
	for(i=0;i<5;i++)
	{
		if(check>num[i])
		{
			check=num[i];
		}
	}
	printf("%d is smallest",check);
}

#WAP TO FIND THE SMALLEST ELEMENT IN AN ARRAY OF SIZE DEFINED BY THE USER
#include<stdio.h>
void main()
{
	int size,i,j,check;
	printf("Enter the size of the array:");
	scanf("%d",&size);
	int num[size];
	printf("Enter the numbers:");
	for(i=0;i<size;i++)
	{
		printf("num[%d]=",i);
		scanf("%d",&num[i]);
	}
	check=num[0];
	for(i=0;i<size;i++)
	{
		if(check>num[i])
		{
			check=num[i];
		}
	}
	printf("%d is smallest",check);
}

#WAP TO INITIALIZE AN ARRAY OF SIZE 5 AND DISPLAY THE LARGEST ELEMENT IN THE ARRAY

#WAP TO FIND THE LARGEST IN AN ARRAY OF SIZE DEFINED BY USER
#include<stdio.h>
void main()
{
	int size,i,j,check;
	printf("Enter the size of the array:");
	scanf("%d",&size);
	int num[size];
	printf("Enter the numbers:");
	for(i=0;i<size;i++)
	{
		printf("num[%d]=",i);
		scanf("%d",&num[i]);
	}
	check=num[0];
	for(i=0;i<size;i++)
	{
		if(check<num[i])
		{
			check=num[i];
		}
	}
	printf("%d is largest",check);
}

#ONE DIMENSIONAL ARRAY SEQUENTIAL SEARCH
-> Basically, sequential search is trying to find an element of the user's interest in an unordered array.
-> ALGORITHM:
Take an unordered non empty array of size n,
Search for the user desired element in the array starting from the first element to the last element.
If there are /are elements that match the user’s searched element then displays those elements.
Else display that “the searched element was not found in the array.”





#WAP Perform Sequential Search in an initialized integer type array for the user desired element.

#include<stdio.h>
int main(){
	int a,b[5]={1,2,3,4,5},i,check=0;
	printf("Enter a number: ");
	scanf("%d",&a);
	for(i=0;i<5;i++){
		if(b[i]==a){
			check++;
		}
	}
	if(check==1)
	{
		printf("Element found");
	}
	else
	{
		printf("Element not found");
	}
	
	return 0;
}


#WAP PERFORM SEQUENTIAL SEARCH IN A USER DEFINED INTEGER TYPE ARRAY OF SIZE N.
#include<stdio.h>
void main()
{
	int size,i,j,check,count=0;
	printf("Enter the size of the array:");
	scanf("%d",&size);
	int num[size];
	printf("Enter the numbers:");
	for(i=0;i<size;i++)
	{
		printf("num[%d]=",i);
		scanf("%d",&num[i]);
	}
	printf("\nEnter the element to be found:");
	scanf("%d",&check);
	for(i=0;i<size;i++)
	{
		if(num[i]==check)
		{
			count++;
		}
	}
	if(count==1)
	{
		printf("Element found");
	}
	else
	{
		printf("NOT found");
	}
}

#SELECTION SORTING (ASCENDING ORDER)
-> Theory: To achieve sorting, two arrays one sorted and another unsorted are used.
-> Mechanism: Array to be sorted is an unsorted array and the sorted array is empty at first. The idea is to start from the start of an array i.e. leftmost location of the array, and compare the item of the first location([0]) with all the items in the array, while comparing the smaller (for ascending order) is kept at consideration for that position([0]) of the array, this smaller value is compared with the value of the next location in the array, so from the 2nd to last comparison, each time the comparison is performed between the value in the correct location and the value obtained from the previous comparison. This process repeats until comparison completes. The value from the final comparison gets swapped with the value of the first position. Now, the first position is the sorted array, again, for the second scan, the same process occurs by taking the value of the 2nd position in the array and performing comparisons as previously done, the value of the final comparison is placed in the second position of the sorted array. 
-> This process keeps on repeating until ((length of array)-1) scan.
-> Algorithm:
	-> Step 1: START
	-> Step 2: Initially the array is regarded as an unsorted array and the sorted array is  empty.
-> Step 3: In this scan, take the left most value from the unsorted list and compare it with
the next value of the unsorted list.
-> Step 4: The smaller value of any comparison is taken as the value to compare to the
next value of the unsorted list.
-> Step 5: This comparison is done until ((number of items in the array)-1) times.
-> Step 6: The value obtained after the final comparison is the smallest in the unsorted
array so is placed in the sorted array and the initial left most value taken before any
comparison is emptied from its place from the unsorted array and is placed in the
unsorted array at the same location where the smallest value was found.
-> Step 7: Until scan is equal to ((number of items in array)-1) Times goto step2.
-> Step 8: Stop.

SOURCE CODE:
#include<stdio.h>
int main (){
    int arr[4]={15,7,38,2};
    int i,j,m,temp,k,num,flag;
    for(j=0;j<3;j++){
    	temp = arr[j];
    	flag = 0;
    	for (i=(j+1);i<4;i++){
    		if(temp>arr[i]){
    			temp=arr[i];
    			k=i;
    			flag=1;
			}
		}
		if (flag==1){
			num=arr[j];
			arr[j]=temp;
			arr[k]=num;
		}
	}
	printf("\n Sorted array in ascending order using selection sort is: \n");
	for (m=0;m<4;m++){
		printf("d\t",arr[m]);
	}
	return 0;

}














#BUBBLE SORTING (ASCENDING ORDER)

-> Theory: To achieve sorting, consecutive two items in the arrays are compared and their locations are swapped if the preceding element is greater.
-> ALGORITHM:
	->STEP 1: Start

	-> Step 2: For every two possible consecutive values in the array from left to
    right, perform comparison between them.

	-> Step 3: If the preceding value of the two values is found to be smaller during
comparison, swapping is performed between them. If there are no swapping at all, then goto step4 else goto step2.

  		-> Step 4: STOP.

Source code:
	#include<stdio.h>

int main(){
		int arr[8] = {1,2,10,5,20,3,5};
		int i,m,temp,flag;
		do{
			flag = 0;
			for(i=0;i<7;i++){
				if(arr[i]>arr[i+1]){
					flag = 1;
					temp = arr[i];
					arr[i] = arr[i+1];
					arr[i+1] = temp;
				}
			}
	} while(flag==1);
		printf("\nThe sorted array using bubble sort in ascending order is:\n");
		for(m=0;m<8;m++){
			printf("%d\t", arr[m]);
	}
		return 0;

}




SOURCE CODE:

#include<stdio.h>
int main(){
	int arr[8]={4,7,3,9,14,12,7,1};
	int i,j,k,l,m,num,temp,flag;
	do{
		flag = 0;
		for (i=0;i<7;i++){
			if (arr[i]<arr[i+1]){
				flag = 1;
				temp= arr[i];
				arr[i]=arr[i+1];
				arr[i+1]=temp;
				
			}
		}
	}
	    while (flag==1);
	    printf ("\n The sorted array using Bubble sort in Ascending order is : \n");
    	for (m=0;m<8;m++){
		
    	printf("%d\t",arr[m]);
		}
	return 0;
}










#Multidimensional array
-Generally, these arrays

 have more than one subscript/dimension and index associated with it.
-These arrays are declared accordingly: 
	Data_type array_name[1][2].....[N]
	where,  N is the nth dimension of the array/

-When the value of N is 2 then this multidimensional array is known as a two dimensional (2-D) array on matrix.

-Even though C allows higher multi-dimensions, most of the multi_dimensional operations are confined mostly to the two dimensional array.

- For example: int arr[4][3][5] refers to array name arr which has 4*3*5=60 integer type data. For instance, this data structure can represent a sales record of an auto-enterprise company in four quarters of 2021 year (quarter 1 to 4) for three location (kathmandu,bhaktapur,lalitpur) and five items(car,bus,jeep,bike,scooter).



  #TWO DIMENSIONAL ARRAY

-In simple, an array that has exactly two subscripts in it is called a two-d array.

-Two-dimensional arrays behave as arrays of one dimensional arrays. Two dimensional array is used mainly for representing data in tabular or matrix form.

-These arrays are declared accordingly:
		Data_type array_name[1][2]

-Where, the first subscript acts as a number of rows and the second subscript acts as the number of columns of a tabular or matrix form data structure.

- example: int arr[2][3] refers to 2 rows and 3 columns, which can also be expressed as 2 arrays each having 3 elements. 

-Accessing the elements of a 2D array can be achieved by using the array name and its corresponding index for both dimensions (Such as: array_name[ith][jth]).


`# Initialization of two-dimensional array

-> Initialization of two dimensional array can be done in several ways:
During initialization comma is used to separate each element and each row are separated by a part of curly braces {} as follows
Int array_name [3] [2] = {{13,8},{10,5},{87,4}};
	Which can also be written as:
Int array_name [3] [2] = {13, 8, 10, 5, 87, 4};

So, from above, it can be said that, the actual dimension depends on the column size of the matrix, which makes it compulsory to mention column size during a declaration, where as the row size is optional such as:
int array_name [] [2] = {13, 8, 10, 5, 87, 4};

It is not advisable to use an incorrect form of declaration as:
Int array_name [ ] [ ] = {13, 8, 10, 5, 87, 4};
Int array_name [5] [ ] ={ 13, 8, 10, 5, 87, 4};

Initialization of two-dimensional array can be done in several ways:
When initializing a zero matrix (all elements are zero):
Int array_name [3] [2] = { {0}, {0}, {0} }, 	// every element in a row gets
                                                                                          Initialized to zero

The elements of an individual matrix array_name [3] [2] = { { 13, 8}, {10, 1}, {33, 9}} is equivalent to :
Array_name[0] [0] = 13;
array_name [0] [1] = 8;
array-name [1] [0] = 10;
array_name [1] [1] = 1;
array_name [2] [0] = 83;
array_name [2] [1] = 9;


# Two Dimensional Example;
Q1. WAP to create, initialize and display 2x2, square matrix.
       # include <stdio.h>

          Int main() {
Int array[2] [2] = { { 7, 5} {3, 4} };
Int row, col;
for( row = 0; row<2; row++){
for( col = 0; col<2; col++) {
printf(“%d\t”, arr(row) (col) );
}
printf(‘\n”)
}
return 0;
}

Q2) WAP to create and display user defined M * N matrix.                          



Practise question :

WAP to find the product of 2  2*2 matrix(User defined)


WAP to find the product of 2  2*2 matrix

#String in C:
#Declaration of strings in C:
#Initialization of Strings in C:
-> Strings can be initialized as:
	Char string_name[4]=”BIM”;
	Char string_name[4]={‘B’,’I’,’M’};
	Char string_name[10]=”BIM FIRST”;
#String literals:
-> In C, within a program at any point in which a value is explicitly specified instead of referring to another variable or some other form of expression, that value is referred to as a literal. In the initialization example below, BIM FIRST is a literal.

Eg: Char string_name[10]= “BIM FIRST”;

-> Thus, it can be said that a string literal is a sequence of characters/ symbolic of the initialization point of the program.

#Reading and Writing strings using scanf and printf
-> Using formatted input function scanf()
	Usage Eg. char str[100];
		scanf(“%s”,str);
-> Using formatted output function printf()
	Usage Eg. printf(“%s”,str);


#WAP TO GET STRING
#include<stdio.h>
void main()
{
	char str[20];
	printf("Enter a word:");
	scanf("%[^\n]",str);
	printf("%s",str);
}

-> Note: scanf() does not read a white space, so reading of character gets terminated after scanf() encounters a white space character i.e. scanf(“%s”,str), where user enters str “BIM FIRST” gets displayed as only BIM. This can be corrected by using conversion character specification %[characters] or %[\characters].
-> %[characters] refers to only the characters written within the big bracket that are allowed as the input of the string. If other than specified characters are encountered, then the reading of characters stops.
-> %[^character]-> refers to when the reading of a character stops when a character after ‘^’ caret symbol is encountered.  

#Reading and writing strings using gets and puts
-> Using unformatted input function gets(), all the characters, including a white space and after white space, are considered as an input. This input functions keeps on reading until a new line character is encountered.
	Usage Eg. Char str[10];
			gets(str);

-> Using unformatted output functions puts(); all the characters are displayed in the screen.
	Usage Eg: puts(str), //str obtained from above example.

#String Manipulation
-> Using string.h header file strings can be:
	-> Checked for its length
	-> Copying of string
	-> Appending the string to another string
	-> Reversing the string.
	-> Comparing two strings 
	-> Changing the cases of the string (upper to lower and vice versa)
          ->Related functions from string.h header files are strlen(),strcat(), strcpy(), strrev(),strcmp(), strwr().

#Some of Built in functions in string.h header file
S.No. 	Function and Description
1		strcpy : copies a string from one variable to another
2		strncpy : copies first n character of one variable to another
3		strlen : finds the length of the string
4		strcat : Attaches/ appends one string at the end of another string
5		strncat :Attaches/ appends first n characters from a string at the end
            of another string.
6		strcmp: Compares two string to check whether they are same or                                                                                                                                                       not.
7		strupr : Converts a string to uppercase.
8		strlute : Converts a string to lowercase.


Example 1: Using strlen()
-> Using strlen(), length of the string (using fgets null character is counted for length, using scanf for string null character is discarded) is returned.

->Syntax:
	Integer_type variable: strlen(string_type variable)

#WAP to display the length of a user defined string.
#include<stdio.h>
#include<string.h>
void main ()
{
	char a[100];
	printf("Enter a string:");
	gets(a);
	printf("\n%s \n%d",a,strlen(a));
}


#WAP TO COPY A INPUT STRING INTO ANOTHER STRING VARIABLE USING BUILT-IN FUNCTIONS.

#include<stdio.h>
#include<string.h>
void main ()
{
	int str[50],str2[50];
	printf("Enter a string:");
	gets(str);
	strcpy(str2,str);
	printf("%s",str2);
}




#EXAMPLE: Concatenate using strcat()
#include<stdio.h>
#include<string.h>
void main ()
{
	char str[50],str2[50],str3[50];
	printf("Enter a string:");
	gets(str);
	strcpy(str2,str);
	printf("%s",str2);
	
	printf("\n%s",strcat(str,str2));
}



#WAP TO CONCATENATE A STRING INPUT IN ONE STRING VARIABLE WITH ANOTHER STRING INPUT IN ANOTHER STRING VARIABLE
#include<stdio.h>
#include<string.h>
void main ()
{
	char str[50],str2[50],str3[50];
	printf("Enter a string:");
	gets(str);
	printf("\nEnter another string:");
	gets(str2);
	printf("\n%s",strcat(str,str2));
}



#EXAMPLE 4: String Comparing using strcmp()
SYNTAX:
	strcmp(string variable1, string variable2);
Returns 0 if both are identical, returns less than 0 if string variable1 is alphabetically smaller than string variable2, returns greater than 0 if string variable1 is alphabetically larger than string variable2.

#WAP TO CHECK WHETHER TWO STRING ARE SAME OR NOT
#include<stdio.h>
#include<string.h>
void main ()
{
	int a;
	char str[50],str2[50],str3[50];
	printf("Enter a string:");
	gets(str);
	printf("\nEnter another string:");
	gets(str2);
	a=strcmp(str,str2);
	printf("%d",a);
	if(a==1)
	{
		printf("Not Same");
	}
	else
	{
		printf("Same");
	}
}


EXAMPLE 5: Reversing a string
Syntax: strrev(string variable)
#include<stdio.h>
Int main(){
	Char str1[10]=”BIM FIRST”;
	printf(“Before reversing:%s”,str1);
	printf(“\n After reversing: %s”,strrev(str1));
}

HOMEWORK: 	strupr()
			strlwr()

HOMEWORK: ALL the programs taught for string.h do it without using built in functions.

FUNCTION:
STRUCTURE OF FUNCTION:
#include<stdio.h>

int add (int, int);

int main(){
	int a,b;
	printf("Enter two nums:");
	scanf("%d %d",&a,&b);
	add(a,b);
	return 0;
}

int add(int x,int y){
	printf("%d",x+y);
}

#USING FUNCTION:
#include<stdio.h>

void mul(int, int);
void sub(int, int);
void add(int, int);
void div(int, int);

int main()
{
	int a,b;
	printf("\n\n\n\tEnter two numbers:");
	printf("\n\n\n\t");
	scanf("%d \t%d",&a,&b);
	system("CLS");
	mul(a,b);
	add(a,b);	
	div(a,b);
	sub(a,b);
	getch();
	system("CLS");
	
	return 0;
}

void mul(int x,int y)
{
	printf("\n\n\n\t%d * %d= %d",x,y,x*y);
}
void add(int x,int y)
{
	printf("\n\t%d + %d= %d",x,y,x+y);
}void div(int x,int y)
{
	printf("\n\t%d / %d= %d",x,y,x/y);
}
void sub(int x,int y)
{
	printf("\n\t%d - %d= %d",x,y,x-y);
}



#NO PARAMETERS
#include<stdio.h>
#define a 5 
#define b 4 
void mul();
void sub();
void add();
void div();

int main()
{
	//printf("\n\n\n\tEnter two numbers:");
	//printf("\n\n\n\t");
	//scanf("%d \t%d",&a,&b);
	system("CLS");
	mul();
	add();
	div();
	sub();
	getch();
	system("CLS");
	
	return 0;
}

void mul()
{
	printf("\n\n\n\t%d * %d= %d",a,b,a*b);
}
void add()
{
	printf("\n\t%d + %d= %d",a,b,a+b);
}void div(int x,int y)
{
	printf("\n\t%d / %d= %d",a,b,a/b);
}
void sub()
{
	printf("\n\t%d - %d= %d",a,b,a-b);
}














