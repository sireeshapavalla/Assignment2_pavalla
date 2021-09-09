# Assignment2_pavalla
a repository of information.
# sireeshapavalla
### Machu Pichu
One of the wonders. it is hill place,**it has ancient history and culture, oldest city **. Embedded within in **dramatic landscape at meeting point between the peruvian**.  
***
# travel dairy's
1. Head east towards wells route
2. Turn right onto  w 2st St
3. Use the right line to take the I-51/US-80 S exit toward US-71 S/Kansas city
4. Keep right  at the road to continue on I29 S
5. Turn right 
    1. Take flight from kansas city airport
    2. Reached charlotte

* Backpack. 
* camera
* Flight Ticket 
* Passport
* cloths

![Link of about me](siripic.jpg)

-----------
# Tables
|The table contains the best food items that are available in charlotte

|Food Items         |Location        |Amount
|---------          |---------       |-------
|thin crust veg     |pls vas         |7$
|cookie crumble     |star bucks      |15$
|chicken spicey     |chick fila      |11$
|avacado veg        |einstein baggles|20$

--------------------

# Pitty Quotes
> The question isn't who is going to let me; it's who is going to stop me
>> A creative man is motivated by the desires to achieve, not by the desire to beat others.

---------

### Code Fencing

> Combinatorics is a branch of mathematics which is about counting - and we will discover many exciting examples of "things you can count,<br>

Source Code: <https://en.wikiversity.org/><br>

// Median and mean

#include<stdio.h>
#include<conio.h>
void main() 
{
int x[100],n,i;
float mean(int,int[]);
float median(int,int[]);
clrscr();
scanf("%d",&n);
for(i=0;i<n;i++)
    scanf("%d",&x[i]);
printf("mean=%f\n",mean(n,x));
printf("median=%f\n",median(n,x));
getch();
}

float mean(int m, int a[]) {
    int sum=0, i;
    for(i=0; i<m; i++)
        sum+=a[i];
    return((float)sum/m);
}


float median(int n, int x[]) {
    int temp;
    int i, j;
    // the following two loops sort the array x in ascending order
    for(i=0; i<n-1; i++) {
        for(j=i+1; j<n; j++) {
            if(x[j] < x[i]) {
                // swap elements
                temp = x[i];
                x[i] = x[j];
                x[j] = temp;
            }
        }
    }

    if(n%2==0) {
        // if there is an even number of elements, return mean of the two elements in the middle
        return((x[n/2] + x[n/2 - 1]) / 2.0);
    } else {
        // else return the element in the middle
        return x[n/2];
    }
}

source code:<https://en.wikiversity.org/wiki/C_Source_Code/Find_the_median_and_mean><br>