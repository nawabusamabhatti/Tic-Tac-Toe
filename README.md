#include <iostream>
using namespace std;
int main()

{
	int x,player,res,select, y[10];
	char name1[32],name2[32];
	char *a,*b,*c,*d,*e,*f,*g,*h,*i;
	char j,k,l,m,n,o,p,q,r;
	a=&j; b=&k; c=&l;d=&m;e=&n;f=&o;g=&p;h=&q;i=&r;
	*a='1';*b='2';*c='3';*d='4';*e='5';*f='6';*g='7';*h='8';*i='9';
	cout<<" !! Tick Cross Game !! \n";
	cout<<"\t- "<<"  - "<<"  -"<<endl<<"\t";
	cout<<*a<<" | "<<*b<<" | "<<*c<<endl;
	cout<<"\t- "<<"  - "<<"  -"<<endl<<"\t";
	cout<<*d<<" | "<<*e<<" | "<<*f<<endl;
	cout<<"\t- "<<"  - "<<"  -"<<endl<<"\t";
	cout<<*g<<" | "<<*h<<" | "<<*i<<endl<<endl<<endl;
	cout<<" Follow Me on Instagram @nawab_usama_bhatti"<<endl;
	cout<<" You Can Also Find Me on Facebook & Twitter as @nawabusamabhati"<<endl<<endl;
	for(int loo=1; loo<10;loo-=-1)
	{
		y[loo]=loo;
	}
	
	
	cout<<"Press 1 To START The Game \n";
	cout<<"Press 2 To EXIT The Game \n";
	re1:
	cout<<"Select ";
	cin>>select;
	if(select==2)
	{
		goto reb;
	}
	else if (select==1)
	{
		goto start;
	}
	else
	{
	cout<<"Invalid Entry Please Enter Again ! \n";
	goto re1;
	}
		start:
		top:
	cout<<"Enter The Name of First Player = ";
	cin>>name1;
	cout<<"Enter The Name of Second Player = ";
	cin>>name2;
	player=1;
		

	do
	{

++player;


	cout<<"\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n     !! Tick Cross Game !! \n";
	cout<<name1<<" ( 'O' )"<<" ~ "<<name2<<" ( 'X' )\n";
	cout<<"\t- "<<"  - "<<"  -"<<endl<<"\t";
	cout<<*a<<" | "<<*b<<" | "<<*c<<endl;
	cout<<"\t- "<<"  - "<<"  -"<<endl<<"\t";
	cout<<*d<<" | "<<*e<<" | "<<*f<<endl;
	cout<<"\t- "<<"  - "<<"  -"<<endl<<"\t";
	cout<<*g<<" | "<<*h<<" | "<<*i<<endl<<endl<<endl;
	ree:
		if(player%2==0)
		{
			
			
			cout<<"it's "<<name1<<"'s Turn !   ";
			rev1:
			cout<<"Enter a Position = ";
			cin>>x;
			if(x<1||x>9)
			{
				cout<<"Invalid Entry ! Please Input Again \n";
				goto rev1;
			}
		}
		else
		{
			
			cout<<"it's "<<name2<<"'s Turn ";
			rev2:
			cout<<"Enter a Position = ";
			cin>>x;
				if(x<1||x>9)
			{
				cout<<"Invalid Entry ! Please Input Again \n";
				goto rev2;
			}
		}
	switch (x)
	{
		case 1:
			y[1]++;
			if(y[1]==2)
			{
			if(player%2==0)
			j='O';
			else
			j='X';
			break;
			}
			else
			{
			cout<<" Position Already Marked Please Select Another \n";
			goto  ree;
			}
		case 2:
			y[2]++;
			if(y[2]==3)
			{
			if(player%2==0)
			k='O';
			else
			k='X';
			break;
			}
			else
			{
			cout<<" Position Already Marked Please Select Another \n";
			goto  ree;
			}
		case 3:
						y[3]++;
			if(y[3]==4)
			{
			if(player%2==0)
			l='O';
			else
			l='X';	
			break;		
				}
			else
			{
			cout<<" Position Already Marked Please Select Another \n";
			goto  ree;
			}
		case 4:
						y[4]++;
			if(y[4]==5)
			{
			if(player%2==0)
			m='O';
			else
			m='X';	
			break;	
				}
			else
			{
			cout<<" Position Already Marked Please Select Another \n";
			goto  ree;
			}	
		case 5:
						y[5]++;
			if(y[5]==6)
			{
			if(player%2==0)
			n='O';
			else
			n='X';	
			break;		
				}
			else
			{
			cout<<" Position Already Marked Please Select Another \n";
			goto  ree;
			}
		case 6:
						y[6]++;
			if(y[6]==7)
			{
			if(player%2==0)
			o='O';
			else
			o='X';	
			break;	
				}
			else
			{
			cout<<" Position Already Marked Please Select Another \n";
			goto  ree;
			}
		case 7:
						y[7]++;
			if(y[7]==8)
			{
			if(player%2==0)
			p='O';
			else
			p='X';			
			break;
				}
			else
			{
			cout<<" Position Already Marked Please Select Another \n";
			goto  ree;
			}
		case 8:
						y[8]++;
			if(y[8]==9)
			{
			if(player%2==0)
			q='O';
			else
			q='X';		
			break;
				}
			else
			{
			cout<<" Position Already Marked Please Select Another \n";
			goto  ree;
			}
		case 9:
						y[9]++;
			if(y[9]==10)
			{
			if(player%2==0)
			r='O';
			else
			r='X';		
			break;	
				}
			else
			{
			cout<<" Position Already Marked Please Select Another \n";
			goto  ree;
			}
	}
	
	

	if(j==k&&k==l)
{
	goto res;
}
	if(m==n&&n==o)
{
	goto res;
}
	if(p==q&&q==r)
{
	goto res;
}
	if(j==m&&m==p)
{
	goto res;
}
	if(k==n&&n==q)
{
	goto res;
}
	if(l==o&&o==r)
{
	goto res;
}
	if(j==n&&n==r)
{
	goto res;
}
	if(p==n&&n==l)
{
	goto res;
}

}while(x!='x');

/* Calculating Result*/

res:
		cout<<"\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n     !! Tick Cross Game !! \n";
	cout<<name1<<" ( 'O' )"<<" ~ "<<name2<<" ( 'X' )\n";
	cout<<"\t- "<<"  - "<<"  -"<<endl<<"\t";
	cout<<*a<<" | "<<*b<<" | "<<*c<<endl;
	cout<<"\t- "<<"  - "<<"  -"<<endl<<"\t";
	cout<<*d<<" | "<<*e<<" | "<<*f<<endl;
	cout<<"\t- "<<"  - "<<"  -"<<endl<<"\t";
	cout<<*g<<" | "<<*h<<" | "<<*i<<endl;
	if(j==k&&k==l)
	{
		if(j=='O')
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name1<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
		
	}
	else
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name2<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	}
		if(m==n&&n==o)
	{
			if(m=='O')
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name1<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	else
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name2<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	}
	if(p==q&&q==r)
	{
	if(p=='O')
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name1<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	else
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name2<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	}

	if(j==m&&m==p)
	{
	if(j=='O')
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name1<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	else
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name2<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	}

	if(k==n&&n==q)
	{
	if(k=='O')
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name1<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	else
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name2<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
}
	if(l==o&&o==r)
{
	if(l=='O')
	{
		cout<<"\n===========================================================\n";
		
		cout<<"Congratulations "<<name1<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	else
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name2<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
}
	if(j==n&&n==r)
{
	if(j=='O')
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name1<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	else
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name2<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
}
		if(p==n&&n==l)
{
	if(p=='O')
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name1<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
	else
	{
		cout<<"\n===========================================================\n";
		cout<<"Congratulations "<<name2<<" You Won The Game ! ";
		cout<<"\n===========================================================\n";
	}
}
re:
cout<<"\n\n Press 1 To Play Again or Press 2 to Exit The Game \n";
cout<<"Select ";
cin>>select;
if(select==1)
{
	
	goto top;
}
else if(select==2)
{
	goto reb;
	
}
else
{
	cout<<"Invalid Entry Please Enter Again ! \n";
	goto re;
}
reb:
	cout<<"Exit ! Thanks For Playing ";


}
