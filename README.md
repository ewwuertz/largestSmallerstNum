# largestSmallerstNum
#include <iostream>
using namespace std;

int main ()
{
int minVal,maxVal;
int array[11]; 
cout<<"This program will ask you to\nenter ten values,";
cout<<"then it will\ndetermine the largest and smallest\nof the values you entered.\n"; 

for(int x=0;x<10;x++)
{
cout<< "\nEnter an integer value: ";
cin>> array[x]; // puts 10 values into array
}

minVal=array[0];
maxVal=array[0];
for(int x=1;x<10;x++)
	{
		if(minVal>array[x])
		{
			minVal=array[x];
		}
		else if(maxVal<array[x])
		{
			maxVal = array[x];
		}
	}
cout<<"\nThe largest value enteted is "<< maxVal << endl;
cout<<"The smallest value entered is "<< minVal << endl;
return 0;
}
