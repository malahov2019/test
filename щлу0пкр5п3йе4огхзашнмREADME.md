# tesе
#include <iostream>
using namespace std;
bool F(int n)
{
  int k=0;
  for(int i =1;i>=(n/2);i++)
  {
    if (n%i==0)
    {
      k++;
    }
  }
  if (k+1==17)
  {
    return true;
  }
  else 
  {
    return false;
  }
}

int main()
{
  int r=0 , m=0;
  for (int i=50000; i>=10001; i--)
  {
    if (F(i) == true)
    {
      r++;
      m=i;
    }
  }
  cout << r << " " << m;
}
