# return_objevt_from_function

#include <bits/stdc++.h>
#include<stdio.h>

using namespace std;
class Student
{
  public:

  int data;
  char name[100];
  char section;
  float mark;

    Student(int x, int s, float m, char*n)
    {
        data=x;
        section=s;
        mark=m;
        strcpy(name,n);
    }
};

Student fun()
{
    //string s;
  // printf("Enter your name::");
    //cin>>s;
    printf("Enter your section::");
    char sec;
    cin>>sec;
    printf("Enter your mark::");
    float mar;
    cin>>mar;
    cout<<"Enter your data::";
    int data;
    cin>>data;

    char s[100]="kausar";
    Student k(data,sec,mar,s);
    return k;


}

int main()
{
    Student kkk=fun();
    cout<<kkk.data<<endl;
    cout<<kkk.section<<endl;
    cout<<kkk.mark<<endl;
    cout<<kkk.name<<endl;



    return 0;
}
