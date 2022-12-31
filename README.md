# stl#include<iostream.h>

#include<conio.h>

#include<stack.h>

#include<queue.h>

#include<map.h>

#include<vector.h>

#include<list.h>

void mystack(){

     stack<int > s1;

     s1.push(5);

     s1.push(10);

     s1.push(15);

     s1.pop();

     s1.size();

     while(!s1.empty()){

	    cout<<s1.top()<<endl;

	    s1.pop();

     }

}

 void myqueue(queue<int> a){

       queue<int> b;

       b=a;

       while(!b.empty()){

	     cout<<b.front()<<endl;

	     b.pop();

       }

}

void mymap(){

    map<int,string> cus;

    cus[100]="hello";

    cus[110]="hii";

    cus[120]="welcome";

    map<int string>:: iteratorp=cus.begin();

    whle(p!=cus.end()){

    cout<<p->second<<endl;

    }

}

 void myvector(){

	vector<int> v1(5,10,15,20);

	cout<<"current capacity="<<v1.capacity();

	v1.push_back(30);

	cout<<"capacity="<<v1.capacity()<<endl;

	vector<int>::iterator p=v1.begin();

	for(i=0;i<v1.size();i++){

		cout<<v1.at(i)<<endl;

	}

       v1.clear();

       cout<<"capacity="<<v1.capacity()<<endl;

}

void mylist(){

    list<int> l1{11,22,33};

    l1.push_back(44);

     list<int>::iterator p=l1.begin;

     while(p!=l1.end()){

	    cout<<*p<<endl;

	    p++;

     }

     l1.pop_back();

     l1.pop_back();

       p=l1.begin;

     while(p!=l1.end()){

	    cout<<*p<<endl;

	    p++;

     }

}

void main(){

	clrscr();

	queue<int> push1;

	push1.push(10);

	push1.push(20);

	push1.push(30);

	myqueue(push1);

	cout<<push1.size();

	cout<<push1.front();

	mystack();

	mymap();

	myvector();

	mylist();

 getch();

}
