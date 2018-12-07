# xudi
c language beginners
/*#include <stdio.h>
#define a1 0
int main()
{
	int a,b,c,d,e,f,g,h,i,j,k,l,m,n,o;
	printf("请输入一个不多于五位数的正整数\n");
	scanf("%d",&a);
	if(a>=0&&a<10){printf("此数一位数\n");
	printf("个位是%10d\n十位是%10d\n百位是%10d\n千位是%10d\n万位是%10d\n",a,a1,a1,a1,a1);
	printf("逆序输出为%6d\n\n",a);}
	else if(a>=10&&a<100){printf("此数二位数\n");b=a/10; f=a%10;
	printf("个位是%10d\n十位是%10d\n百位是%10d\n千位是%10d\n万位是%10d\n",f,b,a1,a1,a1);
	printf("逆序输出为%6d%d\n\n",f,b);}
	else if(a>=100&&a<1000){printf("此数三位数\n");c=a/100; g=a%100%10; h=a%100/10;
	printf("个位是%10d\n十位是%10d\n百位是%10d\n千位是%10d\n万位是%10d\n",g,h,c,a1,a1);
	printf("逆序输出为%6d%d%d\n\n",g,h,c);}
	else if(a>=1000&&a<10000){printf("此数四位数\n");d=a/1000; i=a%1000%100%10;j=a%1000%100/10; k=a%1000/100;
	printf("个位是%10d\n十位是%10d\n百位是%10d\n千位是%10d\n万位是%10d\n",i,j,k,d,a1);
	printf("逆序输出为%6d%d%d%d\n\n",i,j,k,d);}
	else if(a>=10000&&a<100000){printf("此数五位数\n");e=a/10000; l=a%10000%1000%100%10; m=a%10000%1000%100/10;n=a%10000%1000/100; o=a%10000/1000;
	printf("个位是%10d\n十位是%10d\n百位是%10d\n千位是%10d\n万位是%10d\n",l,m,n,o,e);
	printf("逆序输出为%6d%d%d%d%d\n\n",l,m,n,o,e);}
	else if(a>100000){printf("超出范围\n");}

	
}


#include<stdio.h>
int main()
{
	int a,a1;
	int b1=100000*0.1;
	int b2=100000*0.075;
	int b3=100000*0.05;
	int b4=100000*0.03;
	int b5=100000*0.015;
	int b6=100000*0.01;
	printf("输入当月利润");
	scanf("%d",&a);

	if(a<=100000)
	{
		 a1=a*0.1;
	}
	else if(a>100000&&a<=200000)
	{ a1=(a-100000)*0.075+b1;
	}
	else if(a>200000&&a>=400000)
	{ a1=(a-200000)*0.05+b1+b2;
	}
	else if(a>400000&&a<=600000)
	{ a1=(a-400000)*0.03+b1+b2+b3;
	}
	else if(a>600000&&a<=1000000)
	{ a1=(a-600000)*0.015+b1+b2+b3+b4;
	}
	else if(a>1000000)
	{ a1=(a-600000)*0.01+b1+b2+b3+b4+b5;
	}
	printf("总金额为%d",a1);
return 0;
}










#include<stdio.h>
int main()
{
	int a,b;
	double a1;
	double b1=100000*0.1;
	double b2=100000*0.075;
	double b3=100000*0.05;
	double b4=100000*0.03;
	double b5=100000*0.015;
	double b6=100000*0.01;
	printf("输入当月利润");
	scanf("%d",&a);
		if(a<=100000)b=0;
    else if(a>100000&&a<=200000)b=1;
	else if(a>200000&&a>=400000)b=2;
	else if(a>400000&&a<=600000)b=3;
	else if(a>600000&&a<=1000000)b=4;
	else if(a>1000000)b=5;

	switch(b)
	{
	case 0:  a1=a*0.1;break;
	case 1:  a1=(a-100000)*0.075+b1;break;
	case 2:  a1=(a-200000)*0.05+b1+b2;break;
    case 3:  a1=(a-400000)*0.03+b1+b2+b3;break;
	case 4:  a1=(a-600000)*0.015+b1+b2+b3+b4;break;
	case 5:  a1=(a-600000)*0.01+b1+b2+b3+b4+b5;break;
 

	}
	printf("总奖金是%.3f",a1);
return 0;

}*/

/*
#include<stdio.h>           //最大公约数
int main()
{
	unsigned int a,b,c,d,m,n,a1=0;
	printf("请输入正整数\n");
	scanf("%d%d",&m,&n);
	for(a=m;a>0&&a<=m;a-- )
	{
		if(m%a!=0)continue;
		else b=a;
		
		for(c=n;c>0&&c<=n;c--)//
		{
			if(n%c!=0)continue;
			else d=c;
			if(b==d){printf("最大公约数是%d\n",d);a1=1;if(a1==1)break;}
			}
	if(a1==1)	break;}
	printf("最小公倍数是%d\n",m*n/d);
	return 0;
}*/

/*
#include<stdio.h>             //最小公倍数
int main()
{
	int a,b,m,n,i,j,g=0,v;
	printf("请输入正整数\n");
	scanf("%d%d",&m,&n);
	if(m>n){
	a=m;b=n;
	}else{a=n;b=m;}
	for(i=1;i<=b;i++){
	for(j=1,v=1;j<=a;j++,v++){
			if(a*i==b*j){g=1;printf("最小公倍数是%d\n",b*j,a*i);
			if(g==1)break;}
}
	if(g==1){break;}}

return 0;



}*/



/*#include<stdio.h>//4 2 1 循环数
  int main()
{
	unsigned	int a,b,i;
	i=2;
	a=i;
	while(a>1){

	for( ;i>1; )
	{if(i%2==0){
		i/=2;printf("%d  ",i);
		if(i==1){printf("\n\n");}
	}else{
		i=i*3+1;printf("%d  ",i);
	}

	}
	a++;
	i=a;

	}
	return 0;

}*/

/*#include<stdio.h>
  int main()
  {
	 int a[10];
	 int  i,j,t;
	 printf("请输入\n");
	 for(i=0;i<10;i++){
		 scanf("%d",&a[i]);
		 printf("\n");
	 }
	 for(j=0;j<9;j++){
		 for(i=0;i<9-j;i++){
			 if(a[i]<a[i+1]){
			 t=a[i];a[i]=a[i+1];a[i+1]=t;
			 }}
	 
	 }
	 for(i=0;i<10;i++){printf("%d\n",a[i]);}return 0;

  }*/

/*-#include<stdio.h>
int main()
{
	int a[2][3]={{1,2,3},{4,5,6}};
	int b[3][2];
	int i,j;
	printf("a[i][j]为\n");
	for(i=0;i<2;i++){
		
		for(j=0;j<3;j++){
			
			printf(" %d",a[i][j]);b[j][i]=a[i][j];
			if(j==2){printf("\n");}
		}
	}
	printf("b[j][i]为\n");for(j=0;j<3;j++){
		for(i=0;i<2;i++){printf(" %d",b[j][i]);
		if(i==1){printf("\n");}
		}}
	return 0;
}*/

/*
#include<stdio.h>
int main(){
	int a[3][4]={{1,2,3,4},{5,6,7,8},{9,10,11,25}};
	int max;
	int i,j;
	int i1=0,j1=0;
	max=a[0][0];
	for(i=0;i<3;i++){
		for(j=0;j<4;j++){
			if(a[i][j]>max){max=a[i][j];i1=i;j1=j;}

		}
	
	}



	printf("%d\n",a[8][5]);
	printf("max=%d\n位置是第%d行\n第%d列\n",max,i1,j1);
	return 0;




}*/

/*#include<stdio.h>
int main(){
	int i1=1,i2=2,j1=2,j2=3,i3=0,j3=0,con=0;
	double sum1=0.000;
	while(con<20){
		sum1=j1/i1+sum1;
		i3=i1+i2;
		i1=i2;
		i2=i3;

		j3=j1+j2;
		j1=j2;
		j2=j3;
		con++;
		
	}
	printf("  %f\n",sum1);
	return 0;
}*/



#include<stdio.h>
int main(){
	
	int i,j;
	int n0,n1;
	int a[3][3]=
	{{0,1,1},
	{0,1,0},
	{0,0,1}};
	int result=-1;
	int t=0,t1=1;
	int bl,cont=0;
	int b[3][3]={0};


	for(i=0;i<3;i++,cont++){//检查行
	n1=0,n0=0;
		for(j=0;j<3;j++){
		
			if(a[i][j]==0){n0++;}
			else{n1++;}
			if(n1==3){result=1;}
			else if(n0==3){result=0;}
		
			if(cont==2&&result==-1&&j==2){t=1;}//行变列
		if(cont==6){t1=0;break;}
		}
		if(t1==0)break;
		if(t==1){
			for(i=0;i<3;i++){
			for(j=0;j<3;j++){
				
				b[j][i]=a[i][j];
				
				if(i==2&&j==2){for(i=0;i<3;i++){
					for(j=0;j<3;j++){a[i][j]=b[i][j];
					}}}}
			}if(cont==2){i=-1;t=0;};
			}}
	/*if(result==-1){
	for(j=0;j<3;j++){//检查列
		n1=0,n0=0;
		for(i=0;i<3;i++){
		
			if(a[i][j]==0){n0++;}
			else{n1++;}
			if(n1==3){result=1;}
			else if(n0==3){result=0;}
		}
}
	}*/
	printf("%d\n",result);
	printf("  %d %d %d\n  %d %d %d\n  %d %d %d\n",a[0][0],a[0][1],a[0][2],a[1][0],a[1][1],a[1][2],a[2][0],a[2][1],a[2][2]);
	return 0;
}




/*#include<stdio.h>
int main(){
	char a='s';
	int nul=0,shuzi=0,zimu=0,qita=0;
	printf("输入\n");
	
	

	while(a!='\n'){
		scanf("%c",&a);
		if(a==' '){nul++;}
		else if(a>='a'&&a<='z'||a>='A'&&a<='Z'){zimu++;}
		else if(a>='0'&&a<='9'){shuzi++;}
		else qita++;
		
		
	}

	printf("nul=%d\n shuzi=%d\n zimu=%d\n qita=%d",nul,shuzi,zimu,qita);
	return 0;

}*/

/*
#include<stdio.h>
int main(){
	int i,j,k,n;
	for(i=0;i<4;i++){
		for(j=0;j<3-i;j++){printf(" ");}
		for(k=0;k<2*i+1;k++){printf("*");}
		printf("\n");
	}
	for(i=1;i<=3;i++){
		for(j=0;j<i;j++){printf(" ");}
		for(k=0;k<7-2*i;k++){printf("*");}printf("\n");
	}
	printf("\n");//return 0;
//}




//#include<stdio.h>
//int main(){
	//int	i,j,k,n;
	printf("shuruhangshu\n");
	
	//scanf("%d",&n);
	n=4;
	for(i=0;i<n;i++){
		for(j=0;j<n-i;j++){
			if(j<n-1-i)printf(" ");
			else{printf("*");
			if(2*i-1>0){for(k=0;k<2*i-1;k++){
				printf(" ");if(k==2*i-2){printf("*\n");}
			}}else printf("\n");
			}
		}
	}for(i=1;i<n;i++)
		for(j=0;j<i+1;j++){
			if(j<i)printf(" ");
			else {
				printf("*");for(k=0;k<2*(n-i-1)-1;k++){
					printf(" ");if(k==2*(n-i-1)-2)printf("*\n");
				}}
		}
	
		printf("\n");


	return 0;
}*/

//#include<stdio.h>
//int main(){
//	char a[][7]={{"   *   "},};
//
//}




//
//#include<stdio.h>           //最大公约数
//int main(){
//	int max(int	m,int n);
//	int min(int m,int n);
//	int d,c,a,b;
//	scanf("%d%d",&a,&b);
//	c=max(a,b);
//	d=min(a,b);
//	printf("%d,%d",c,d);
//	return 0;
//
//}
//
//int min(int m,int n)
//{
//	int a;
//	int max(int m,int n);
//	a=m*n/(max(m,n));
//	return a;
//
//}
//
//int max(int	m,int n)
//{
//	unsigned int a,b,c,d,a1=0;
//	
//	
//	for(a=m;a>0&&a<=m;a-- )
//	{
//		if(m%a!=0)continue;
//		else b=a;
//		
//		for(c=n;c>0&&c<=n;c--)
//		{
//			if(n%c!=0)continue;
//			else d=c;
//			if(b==d){a1=1;if(a1==1)break;}
//			}
//	if(a1==1)	break;}
//	return (d);
//	}

//

#include<stdio.h>
int main() {
	int	i = 1, j = 1, k;
	int a, b, c, d;
	//a = 10;
	//b = a++;
	//c = ++a;
	//d = 10 * a++;
	k = (j++)+(++j)+(++j)+(++j);
	//a = i++;
	//b = i++;
	//c = i++;
	//d = a+b+c;
	
	printf("%d %d ",k,j);
	return	0;

}
