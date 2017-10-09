#include <iostream>
#include <fstream> 
#include <cmath> 
using namespace std;

void polar (float x, float y, float &r, float &theta);

int main (void)
{
    
    float x, y, r, theta;
    
    ifstream fin ("polar.txt");
    ofstream fout ("polarout.txt");
    
    while (fin >> x >> y ) {
    polar(x,y,r,theta);
    
    
    fout << r << " " << theta << endl;
}
   
    fin.close();
    fout.close();
    return 0;
}

void polar (float x, float y, float &r, float &theta)
{

   r = sqrt(x*x + y*y);
   if(r>0 && y > 0){
    theta = acos(x/r);  
	    }
	
	else if(r>0 && y <= 0){
           theta = -acos(x/r);  
		     }
		   
		   
		   else{
               theta = 0;      }
                      
     }
