#include<iostream>
using namespace std;
#define size 5

class stack
{
   int stack[size];
   int top;
   
   public:
   void init();
   void push(int i);
   int pop();
   void display();
   int peek();
 };
 
 void stack::init()
 {
    top=0;
 }
  
  void stack::push(int i)
  {
      
      if (top==size-1)
      {
       cout<<"Stack Overflow";
       return;
       }
       
       stack[top]=i;
       top++;
  }
  
  int stack::pop()
  {
     if (top==0)
     {
         cout<<"Stack Underflow";
         return 0;
      }
      top--;
      cout<<"The Popped Element is:\n"<<stack[top];
  }
  
 void stack::display()
 {
     int i;
     if(top==0)
     {
         cout<<"Stack Empty";
      }
      cout<<"\n Printing Elements:\n";
      for(i=0;i<top;i++)
      {
           cout<<stack[i];
           cout<<"\n";
       }
  }
  
  int stack::peek()
  {
   cout<< "\n The Top Element is:\n";
   cout<<stack[top];
   }
  
  int main()
  {
       int ch;
       stack s;
       s.init();
       
       s.push(4);
       s.push(3);
       s.push(2);
       s.display();
       s.pop();
       s.display();
              

                    
}            
