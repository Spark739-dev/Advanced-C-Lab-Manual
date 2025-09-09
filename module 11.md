

## EXP NO:21 C PROGRAM TO CREATE A FUNCTION TO FIND THE GREATEST NUMBER
## Aim:
To write a C program to create a function to find the greatest number

## Algorithm:
1.	Include the necessary header #include <stdio.h>.
2.	Use a series of if and else if statements to compare the values and return the maximum among them.
3.	Declare variables n1, n2, n3, n4, and greater to store user input and the result.
4.	Use scanf to take four integers as input.
5.	Call the max_of_four function with the input integers and store the result in the greater variable
 
## Program:
     #include<stdio.h>
     int max_of_four(int a,int b,int c,int d)
     {
         if(a>b && a>c && a>d)
         {
             return a;
             
         }
         else if(b>a && b>c && b>d)
         {
             return b;
             
         }
         else if(c>a && c>b && c>d)
         {
             return c;
             
         }
         else
         {
             return d;
             
         }
         
     }
     int main()
     {
         int n1,n2,n3,n4,greater;
         scanf("%d%d%d%d",&n1,&n2,&n3,&n4); 
         greater=max_of_four(n1,n2,n3,n4);
         printf("%d",greater);
     }

## Output:
<img width="206" height="274" alt="image" src="https://github.com/user-attachments/assets/4caca140-9d2c-4ace-94d2-3f93c2471771" />


## Result:
Thus, the program  that create a function to find the greatest number is verified successfully.


 
## EXP NO:22 C PROGRAM TO PRINT THE MAXIMUM VALUES FOR THE AND, OR AND  XOR COMPARISONS
## Aim:
To write a C program to print the maximum values for the AND, OR and XOR comparisons

## Algorithm:
1.	Define a function calculate_the_max that takes two integers n and k as parameters.
2.	Declare variables a, o, and x to store the maximum values for AND, OR, and XOR operations, respectively.
3.	Use nested loops to iterate through pairs of integers (i, j) from 1 to n.
4.	Within the loops, check conditions for AND, OR, and XOR operations and update the corresponding maximum values (a, o, x).
5.	Declare variables n and k to store user input.
6.	Use scanf to take two integers as input.
7.	Call the calculate_the_max function with input values.
 
## Program:
    #include <stdio.h>
    void comp(int n, int k) {
        int max_and = 0;
        int max_or = 0;
        int max_xor = 0;
        for (int i = 1; i <= n; i++) {
            for (int j = i + 1; j <= n; j++) {
                int and_value = i & j;
                int or_value = i | j;
                int xor_value = i ^ j;
                if (and_value < k) {
                    if (and_value > max_and) {
                        max_and = and_value;
                    }
                }
    
                if (or_value < k) {
                    if (or_value > max_or) {
                        max_or = or_value;
                    }
                }
                if (xor_value < k) {
                    if (xor_value > max_xor) {
                        max_xor = xor_value;
                    }
                }
            }
        }
        printf("%d\n", max_and);
        printf("%d\n", max_or);
        printf("%d\n", max_xor);
    }
    
    int main() {
        int n, k;
        scanf("%d %d", &n, &k);
        comp(n, k);
        return 0;
    }

## Output:
<img width="297" height="314" alt="image" src="https://github.com/user-attachments/assets/a167443d-7bf0-4c5b-b269-2413ddc324cd" />

## Result:
Thus, the program to print the maximum values for the AND, OR and XOR comparisons
is verified successfully.


 
## EXP NO:23 C PROGRAM TO WRITE THE LOGIC FOR THE REQUESTS
## Aim:
To write a C program to write the logic for the requests

## Algorithm:
1.	Declare variables noshel and noque to store the number of shelves and the number of queries, respectively.
2.	Use scanf to take two integers as input for the number of shelves and queries.
3.	Declare a 2D array shelarr to represent shelves and books, and an array nobookarr to store the number of books on each shelf.
4.	Declare variables k and c to keep track of the book index and the total number of books.
5.	Use a for loop to iterate over the queries.
 
## Program:
    #include <stdio.h>
    int main(){
        int total_number_of_shelves;
        int total_number_of_queries; 
        scanf("%d",&total_number_of_shelves);
        scanf("%d",&total_number_of_queries); 
        int total_number_of_books[1000]={0};
        int total_number_of_pages[1000][1100]; 
        while(total_number_of_queries--){
            int type;
            scanf("%d",&type);
            if(type==1){
                int x,y;
                scanf("%d %d",&x,&y);
                total_number_of_pages[x][total_number_of_books[x]]=y;
                total_number_of_books[x]++;
            }
            else if(type==2){
                int x,y;
                scanf("%d %d",&x,&y);
                printf("%d\n",total_number_of_pages[x][y]);
            } else if(type==3){
                int x;
                scanf("%d",&x);
                printf("%d\n",total_number_of_books[x]); 
            }
        }
    }

## Output:
<img width="324" height="182" alt="image" src="https://github.com/user-attachments/assets/ee0897e4-9038-4897-b988-390895364c36" />



## Result:
Thus, the program to write the logic for the requests is verified successfully.


 
## EXP NO:24 C PROGRAM PRINT THE SUM OF THE INTEGERS IN THE ARRAY.
## Aim:
To write a C program print the sum of the integers in the array.

## Algorithm:
1.	Declare a variable n to store the number of integers.
2.	Use scanf to take an integer n as input.
3.	Declare an array a of size n to store the integers.
4.	Declare a variable sum and initialize it to zero.
5.	Use a for loop to iterate n times:
6.	Use scanf to input each integer and add it to the sum.
7.	Print the final sum using printf.



## Program:
    #include<stdio.h>
    int main()
    {
        int n; scanf("%d",&n);
        int a[n];
        int sum=0;
        for(int i=0;i<n;i++)
        {
            scanf("%d",&a[i]);
            sum=sum+a[i];
            
        }
        printf("%d",sum);
    }

## Output:


 <img width="346" height="169" alt="image" src="https://github.com/user-attachments/assets/83629168-4ed9-40dd-9d8e-c7943743a2ee" />



## Result:
Thus, the program prints the sum of the integers in the array is verified successfully.


 
## EXP NO 25: C PROGRAM TO COUNT THE NUMBER OF WORDS IN A      SENTENCE



## Aim:

To write a C program that counts the number of words in a given sentence.

## Algorithm:

1.	Input the sentence: Take a sentence from the user.
2.	Initialize a counter variable: This will keep track of the number of words.
3.	Process each character of the sentence:
o	Iterate through the sentence, checking each character.
o	If a character is not a space, it may belong to a word. If it's the first non-space character after a space or at the start, increment the word count.
4.	Handle spaces and punctuation: Skip over spaces, punctuation marks, and consider each word as a sequence of characters separated by spaces.
5.	Display the result: After processing the sentence, output the total word count.



## Program:
     #include<stdio.h>
     #include<string.h>
     int main()
     {
         char str[100];
         fgets(str,sizeof(str),stdin);
         int len=sizeof(str);
         int count=1;
          for(int i=0;i<len-1;i++){
              if(str[i]==' ')
              count++;
              
          }
          printf("Total number of words in the string is :%d",count);
         return 0;
     }

## Output:
<img width="945" height="175" alt="image" src="https://github.com/user-attachments/assets/3ad27241-6d65-4e02-8fee-79ed9b48e76e" />



## Result:

Thus, the program that counts the number of words in a given sentence is verified 
successfully.
