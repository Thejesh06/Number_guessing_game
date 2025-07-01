#include<bits/stdc++.h>
using namespace std;
int main()
{
    int cnt;
    string s;
    do{
    int n;
    srand((long int)clock());
    int num=rand()%100;
    cnt=0;
    do{
    cout<<"Guess a number b/w 1 and 100: ";
    cin>>n;
    cnt++;
    if(n>num)cout<<"Too high"<<endl;
    else if(n<num)cout<<"Too low"<<endl;
    else
    cout<<"correct!"<<endl;
    }   while(n!=num);
    cout<<"No of guesses: "<<cnt<<endl;
    cout<<"Do u want to continue (yes/no): ";
    cin>>s;
    }
    while(s=="yes");
    
    return 0;

    
}