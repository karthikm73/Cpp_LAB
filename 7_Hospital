//hospital data base
#include <iostream>
using namespace std;
struct date
{
	int d;
	int m;
	int y;
};
class hospital
{
	char name[100];
	struct date d_adm;
	struct date d_dis;
	protected : 
	int age;
	public:
	void getdata()
	{
		cout<<"Enter name of patient: ";
		cin>>name;
		cout<<"Enter age: ";
		cin>>age;
		cout<<"Enter date of admission: ";
		cin>>d_adm.d>>d_adm.m>>d_adm.y;
		cout<<"Enter date of discharge: ";
		cin>>d_dis.d>>d_dis.m>>d_dis.y;
	}
	void display()
	{
		cout<<name<<"\t";
		cout<<age<<"\t";
		cout<<d_adm.d<<"-"<<d_adm.m<<"-"<<d_adm.y<<"\t \t \t";
		cout<<d_dis.d<<"-"<<d_dis.m<<"-"<<d_dis.y;
	}
};
class pediatric_patient: public hospital
{
	char vaccine[20];
	public:
	void get()
	{
		getdata();
		cout<<"enter name of vaccine to be given: ";
		cin>>vaccine;
	}
	void put()
	{
		if(age<12)
		{
			display();
			cout<<"\t\t\t\t"<<vaccine<<endl;
		}
		else
			cout<<"age is greater than 12, not a pediatric patient"<<endl;
	}
};

int main()
{
	hospital h[5];
	int n;
	cout<<"Enter number of patients: ";
	cin>>n;
	for(int i=0;i<n;i++)
	{
		h[i].getdata();
	}
	cout<<"Patient database: "<<endl;
	cout<<"NAME\tAGE\tDATE_OF_ADMISSION\tDATE_OF_DISCHARGE\n";
	for(int i=0;i<n;i++)
	{
		h[i].display();
		cout<<endl;
	}
	pediatric_patient a1[5];
	cout<<"Enter number of pediatric patients: ";
	cin>>n;
	for(int i=0;i<n;i++)
	{
		a1[i].get();
	}
	cout<<"Pediatric patient database: "<<endl;
	cout<<"NAME\tAGE\tDATE_OF_ADMISSION\tDATE_OF_DISCHARGE\tVACCINE\n";
	for(int i=0;i<n;i++)
	{
		a1[i].put();
	}
	return 0;
}
