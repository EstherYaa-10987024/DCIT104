
#include<iostream> 
using namespace std; 



// Name: Esther Kumah



// ID: 10987024
  
bool isPrime(int n); 
  
int main() 
{   
  int num, sum=0, count=0; 
     
     cout<<"Enter the number: "; 
     cin>>num; 
      
  for(int j=0; count<num; j++) 
  { 
    if(isPrime(j))  
    { 
      sum += j; 
      count++;   
    } 
  } 
   
  cout<<"The average of the first "<<num<<" prime numbers are "<<(float)sum/count; 
} 
  
bool isPrime(int n) 
{ 
  bool flag = true; 
   
  if (n<2)    flag = false; 
  else if(n==2)  flag = true; 
  else 
  { 
    for(int i=2; i<=n/2; i++) 
    { 
      if(n%i==0) 
      { 
        flag = false; 
        break; 
      } 
    } 
  }   
  return flag;   
}
