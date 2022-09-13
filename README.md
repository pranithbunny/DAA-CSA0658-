#include<stdio.h>
int main()
{
	int i,n,low,mid,high,search,arr[100];
	printf("enter the number of elements");
	scanf("%d",&n);
	printf("enter %d elements",n);
	for(i=0;i<n;i++)
	scanf("%d",&arr[i]);
	printf("enter the searching element");
	scanf("%d",&search);
	low=0;
	high=n-1;
	mid=(low+high)/2;
	while(low<=high)
	{
			mid=(low+high)/2;
	if(arr[mid]<search)
	low=mid+1;
	else if(arr[mid]==search)
	{
		printf("%d found at location %d",search,mid+1);
		break;
	}
	else 
	high=mid-1;

}
if(low>high)
printf("%d element not found ",search);
return 0;	
}
