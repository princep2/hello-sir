# hello-sir   // I AM PRINCE PRAFULL FROM DELHI PUBLIC SCHOLL GREATER NOIDA
Static Stack

#include<iostream.h>
#include<conio.h>

struct node
{
  int info;
  node *next;
 }*ptr,*np,*start,*save;
 
 node *create(int ele)
 {
   ptr=new node;
   ptr->info=ele;
   ptr->next=NULL;
   return ptr;
  }
  
  void push(node *np)
  {
    if(start==NULL)
    start=np;
    else
    {
      save=start;
      start=ptr;
      ptr->next=save;
     }
    }
    
    void pop()
    { 
      if(start==NUll)
      cout<<"overflow";
      else
      {
        ptr=start;
        star=ptr->next;
        delete ptr;
       }
     }
     
     void disp(node * np)
     {
       while(ptr!=NULL)
       {
         cout<<ptr->info;
         ptr=ptr->next;
        }
       }
       
       int main()
       {
         clrscr();
         int ele;
         cin>>ele;
         np=create(ele);
         push(np);
         pop();
         disp(np);
         getch();
        } 
       


repository
