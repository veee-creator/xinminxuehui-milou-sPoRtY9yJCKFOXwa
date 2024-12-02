
# [题目传送门](https://github.com)


## 思路


首先看一下数据范围。


* 1≤N,M≤2×105
* 1≤Ai,Bi≤2×105


这么大的数据范围肯定不能直接写二重循环暴力。




---


考虑一下，应为它是从每个人面前顺序经过的。那我们就可以按照顺序，依次枚举这 N 个人。
首先记录这些食物对应的序号，再的按照美味度从小到大排序。
依次枚举这 N 个人，只要发现一个不小于他的品味值的食物，就给这个食物打上标记，同时指针往前移一位。
如果所有的食物都已经被打上了标记，就提前跳出循环。
否则到最后的时候，就按照标记输出，如果这个食物没有被打上标记，就输出 `-1`。


## 代码



```
#include
using namespace std;
struct no
{
	int x,y;
}h[1000000];
int cmp(no q,no w)
{
	return q.xint hh[1000000];
int a[1000000];
int main()
{
	ios::sync_with_stdio(false);
	cin.tie(),cout.tie();
	int n,m;
	cin>>n>>m;
	for(int i=1;i<=n;i++)
		cin>>a[i];
	for(int i=1;i<=m;i++)
	{
		cin>>h[i].x;
		h[i].y=i;
	}
	sort(h+1,h+m+1,cmp);
	int x=m+1;
//	for(int i=1;i<=m;i++)
//	cout<
//	cout<
//	for(int i=1;i<=m;i++)
//	cout<
	for(int i=1;i<=n;i++)
	{
		if(x==0)
			break;
		while(1)
		{
			x--;
			if(h[x].x>=a[i])
			{
				hh[h[x].y]=i;
			}
			else
			{
				x++;
				break;
			}
		}
	}
	for(int i=1;i<=m;i++)
	{
		if(hh[i]==0)
		cout<<-1;
		else
		cout<
```

 本博客参考[slower加速器官网](https://chundaotian.com)。转载请注明出处！
