# mastercodes
C++ in class
bu classda o'zingiz haqingizda ma'lumot olasiz.
#include<bits/stdc++.h>
using namespace std;
class student{
	public:
		string ism;
		string familiya;
		int yosh;
		string manzili;
		string kasbi;
		int kurs;
		double gpa;
	 student(string ism,string familiya,int yosh,string manzili,string kasbi,int kurs,double gpa){
	 	this->ism=ism;
	 	this->familiya=familiya;
	 	this->yosh=yosh;
	 	this->manzili=manzili;
	 	this->kasbi=kasbi;
	 	this->kurs=kurs;
	 	this->gpa=gpa;
	 }  
	 void display(){
	 	cout<<"Ismi: "<<ism<<endl;
	 	cout<<"Familiyasi: "<<familiya<<endl;
	 	cout<<"yosh: "<<yosh<<endl;
	 	cout<<"manzili: "<<manzili<<endl;
	 	cout<<"kasbi: "<<kasbi<<endl;
	 	cout<<"kurs: "<<kurs<<endl;
	 	cout<<"Gpa ball: "<<gpa<<endl;
	 }  
	 void set_ism(string ism){
	 	this->ism=ism;
	 }
	 void set_familiya(string familiya){
	 	this->familiya=familiya;
	 }
	 void set_yosh(int yosh){
	 	this->yosh=yosh;
	 }
	 void set_manzili(string manzili){
	 	this->manzili=manzili;
	 }
	 void set_kasbi(string kasbi){
	 	this->kasbi=kasbi;
	 }
	 void set_kursi(int kursi){
	 	this->kurs=kursi;
	 }
	 void set_gpa(double gpa){
	 	this->gpa=gpa;
	 }
};
int main(){
 student s("Izzabek","Abdusharipov",21,"Kharezm","student",2,5);
	cout<<"Ismingizni kiriting: ";
	string name;
	cin>>name;
	s.set_ism(name);
	
	cout<<"Familiyangizni kiriting: ";
	string surname;
	cin>>surname;
	s.set_familiya(surname);
	
	cout<<"Yoshingizni kiriting: ";
	int age;
	cin>>age;
	s.set_yosh(age);
	
	cout<<"Manzilingizni kiriting: ";
	string address;
	cin>>address;
	s.set_manzili(address);
	
	cout<<"Kasbingizni kiriting: ";
	string job;
	cin>>job;
	s.set_kasbi(job);
	
	cout<<"Kursingizni kiriting: ";
	int course;
	cin>>course;
	s.set_kursi(course);
	
	cout<<"GPA balingizni kiriting: ";
	double gpa;
	cin>>gpa;
	s.set_gpa(gpa);
	s.display();
	
	return 0;
}
