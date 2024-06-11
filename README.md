# convert these times into seconds 
 a program in which user enter 2 times in (hh:mm:ss) you have to convert these times into seconds and add them and then again convert the total seconds back into (hh:mm:ss) format.
 #include<iostream>
using namespace std;
struct time
{
int hour;
int min;
int sec;
};
int main()
{
time t1,t2,t3;
int sec1,sec2,tsec;
cout<<"enter time in hh:mm:ss this format"<<endl;
cin>>t1.hour>>t1.min>>t1.sec;
cout<<"enter time in hh:mm:ss this format"<<endl;
cin>>t2.hour>>t2.min>>t2.sec;
sec1=t1.hour*3600+t1.min*60+t1.sec;
sec2=t2.hour*3600+t2.min*60+t2.sec;
tsec=sec1+sec2;
t3.hour=tsec/3600;
t3.min=(tsec%3600)/60;
t3.sec=(tsec%3600)%60;
cout<<"Time ="<<t3.hour<<":"<<t3.min<<":"<<t3.sec;
return 0;
}
