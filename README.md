#include <iostream>
#include <stdlib.h> 
#include <time.h>  
using namespace std;
int main() 
{
   cout<<"************************************************"<<endl;
   cout<<"*        欢迎使用学生成绩管理系统1.1           *"<<endl;
   cout<<"*        小组14   计算机2003班 2020.10.29      *"<<endl;
   cout<<"*        1、输入4位同学的代号和成绩            *"<<endl;
   cout<<"*        2、显示4位同学的代号和成绩列表        *"<<endl;
   cout<<"*        3、求4人平均分                        *"<<endl;
   cout<<"*        4、求4人总分                          *"<<endl;
   cout<<"*        5、查询某同学的分数                   *"<<endl;
   cout<<"*        6、统计及格率                         *"<<endl;
   cout<<"*        7、退出                               *"<<endl;
   cout<<"*        输入（1-7）进行选择                   *"<<endl;
   cout<<"************************************************"<<endl;
   cout<<"     "<<endl;
   float z,a,b,c,d;
   double f;
   char e;
   int x;
cout<<"请先分别输入4位同学的成绩"<<endl;
cin>>a>>b>>c>>d;
cout<<"请选择功能(1-7):";
cin>>x; 
 switch(x)
 {
	case 1:
	cout<<"输入4个人的代号和成绩"<<endl;
    char u,i,o,p;
    cout<<"先分别输入代号："<<endl;
	cin>>u>>i>>o>>p;
	cout<<"输入成绩："<<endl;
	cin>>a>>b>>c>>d;
	break;
	case 2:cout<<"4位同学的代号和成绩分别为："<<endl;
		       cout<<"同学A:"<<"代号为A，成绩为"<<a<<endl; 
		       cout<<"同学B:"<<"代号为B，成绩为"<<b<<endl; 
		       cout<<"同学C:"<<"代号为C，成绩为"<<c<<endl; 
		       cout<<"同学D:"<<"代号为D，成绩为"<<d<<endl; 
		       break;
          case 3:z=(a+b+c+d)/4;
		       cout<<"4人平均分为: "<<z<<endl;
		       break;

		case 4: 
		cout<<"4人总分为："<<a+b+c+d; break;
		case 5: 
		cout<<"查询某同学的分数：";
		cin>>e;
		switch(e)
		{
			case 'A': cout<<"A同学的成绩是"<<a; break;
			case 'B': cout<<"B同学的成绩是"<<b; break;
			case 'C': cout<<"C同学的成绩是"<<c; break;
			case 'D': cout<<"D同学的成绩是"<<d; break;
		}
		break;
		case 6: 
		cout<<"统计及格率：";
		f=0;
		if(a>=60)
		f=f+1;
		if(b>=60)
		f=f+1;
		if(c>=60)
		f=f+1;
		if(d>=60)
		f=f+1;
		cout<<(f/4)*100<<"%";
		break;
	    case 7:break;
		  }
        return 0;}

