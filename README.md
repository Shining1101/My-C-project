# My-C-project
C++ overloaded operators and overloaded functions
C++ allows multiple definitions of a function and operator in the same scope, called function overloading and operator overloading, respectively.
#include <iostream>
using namespace std;

class printData
{
   public:
      void print(int i) {
        cout  << i << endl;
      }

      void print(double  f) {
        cout <<  f << endl;
      }

      void print(char c[]) {
        cout << c << endl;
      }
};

int main(void)
{
   printData pd;

   pd.print(5);
  
   pd.print(500.263);
   
   char c[] = "Hello C++";
   pd.print(c);

   return 0;
}
