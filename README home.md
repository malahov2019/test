# test
#include <iostream>
using namespace std;
int F(int n)
{
  if (n==0)
    return 0;
  if ((n>0) && (n%2==0))
    return F(n/2);
  if ((n>0) && (n%2!=0))
    return 1+F(n-1);
}

int main()
{
  int n;
  for (int i=0; i<1000000; i++)
  {
    n=i;
    if (F(n)==12)
    {
      cout << i;
      break;
    }
  }
}
