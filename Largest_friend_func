//2b)



#include<iostream>
using namespace std;

class Test {
private:
   int x, y, z;
public:

   void input() {
       cout << "Enter three numbers:";
       cin >> x >> y>>z;
   }

   friend void find(Test t);
};

void find(Test t) {
   if (t.x > t.y && t.x > t.z) {
       cout << "Largest is:" << t.x;
   } else if (t.y > t.z) {
       cout << "Largest is:" << t.y;
   } else {
       cout << "Largest is:" << t.z;
   }
}

int main() {
   Test t;
   t.input();

   find(t);
   return 0;
}
