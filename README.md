# patterncode

#include <iostream>

using namespace std;
void
triangle (int n)
{
  // number of spaces
  int k = 2 * n - 2;
  for (int i = 0; i < n; i++)
    {
      for (int j = 0; j < k; j++)
	cout << " ";

      k = k - 1;

      for (int j = 0; j <= i; j++)
	{
	  if (i == 0)
	    {
	      cout << "* ";
	    }
	  else if (i % 4 == 1)
	    {
	      cout << "+ ";
	    }
	  else if (i % 4 == 2)
	    {
	      cout << "- ";
	    }

	  else if (i % 4 == 3)
	    {
	      cout << "/ ";
	    }

	  else if (i % 4 == 0)
	    {
	      cout << "* ";
	    }

	}

      cout << endl;
    }
}

int
main ()
{
  int n = 4;
  
  if(n%4 ==0 ){

  design (n);}
  else{
      cout<<"enter valid value ";
  }
  return 0;
}
