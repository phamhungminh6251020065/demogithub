# demogithub
#include<iostream>
#include<math.h>
using namespace std;
int main(){
	float a, b, c, delta, x1,x2;
	cout<<"Nhap a, b, c: ";
	cin>>a>>b>>c;
	if(a==0)
		cout<<"PT nay khong phai la phuong trinh bac hai";
	else{
		delta=b*b-4*a*c;
		if(delta<0)
			cout<<"PTVN";
		else if(delta==0){
			x1=-b/(2*a);
			cout<<"Nghiem la: "<<x1;
		}
		else{
			x1=(-b+sqrt(delta))/(2*a);
			x2=(-b-sqrt(delta))/(2*a);
			cout<<"x1 = "<<x1<<" va x2 = "<<x2;
		}
	}
}
