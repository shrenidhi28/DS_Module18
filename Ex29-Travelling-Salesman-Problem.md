# Ex29 Travelling Salesman Problem
## DATE: 12-05-25
## AIM:
To write a C Program to implement Travelling Salesman Problem for finding shortest path.
## Algorithm:


## Program:
```
/*
Program to implement Travelling Salesman Problem for finding shortest path
Developed by:  C.Shrenidhi
RegisterNumber:  212223040196
*/
#include<stdio.h>
int a[10][10],visited[10],n,cost=0;
void get()
{
int i,j;
scanf("%d",&n);
for(i=0;i < n;i++)
{
for( j=0;j < n;j++)
scanf("%d",&a[i][j]);
visited[i]=0;
}
}
void mincost(int city)
{
int ncity;
int least(int);
visited[city]=1;
printf("%d -->",city+1);
ncity=least(city);
if(ncity==999)
{
}
ncity=0;
printf("%d",ncity+1);
cost+=a[city][ncity];
return;
mincost(ncity);
}
{
int least(int c)
int i,nc=999;
int min=999,kmin;
for(i=0;i < n;i++)
{
if((a[c][i]!=0)&&(visited[i]==0))
if(a[c][i] < min)
{
min=a[i][0]+a[c][i];
kmin=a[c][i];
nc=i;
}
}
if(min!=999)
cost+=kmin;
return nc;
}
void put()
{
}
int main()
{
get();
mincost(0);
put();
return 0;
}
printf("\n\nMinimum cost:%d",cost);
```

## Output:

<img width="287" alt="image" src="https://github.com/user-attachments/assets/5f9721bc-2c7c-4701-b252-125ec4486ee1" />




## Result:
Thus, the C program to implement Travelling Salesman Problem for finding shortest path is implemented successfully.
