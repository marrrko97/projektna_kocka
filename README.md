#include <iostream>
#include <stdlib.h>
#include <ctime>
#include <math.h>
using namespace std;

int main()
{
	int random;
	int x=0;
	int y=0;
	int a=0; 
	double razdalja;
	
	srand(time(0));
	
	cout << "Vpisi kolikokrat zelis metat kocko:  ";
	cin >> a;
	cout << endl; 
	
	for(int j=0; j<50; j++)
	{
	for(int i=0; i<a; i++)
	{
					
	random = rand() %4 + 1;	
	
	if(random==1)
	{
	 x++;
	cout << "kocka: " << random << endl;
	cout << "x= " << x << endl << endl ; 
	}
		if(random==2)
	{
	 y++;
	 cout << "kocka: " << random << endl;
	 cout << "y= " << y << endl << endl ;
	}
		if(random==3)
	{
	 x--;
	 cout << "kocka: " << random << endl;
	 cout << "x= " << x << endl << endl ;
	}
		if(random==4)
	{
	 y--;
	 cout << "kocka: " << random << endl; 
	 cout << "y= " << y << endl << endl ;
	}
		
			
}

cout << "razdalja je: " << razdalja << endl;
razdalja = sqrt(x*x+y*y);

}
	return (0);
}
