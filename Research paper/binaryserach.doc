#include<stdio.h>

int BS(int [],int ,int ,int);
int main()
{
	int arr[]={1,3,5,7,9,11,12};
	int i,j,key,pos;
	i=0;
	j=sizeof(arr)/sizeof(arr[0])-1;
	printf("Enter the key which is to be search=");
	scanf("%d",&key);
	
	
	pos=BS(arr,i,j,key);
	if(pos!=-1)
	printf("Key is found at the position %d",pos+1);
	else
	printf("Key is not found");
	return 0;
}
BS(int arr[],int i,int j,int key)
{
	int mid;
	if(i==j)
	{
		if(key==arr[i])
		return i;
		else
		return -1;
	}
	else
	{
	mid=i=(j-i)/2;
	if(arr[mid]==key)
	return mid;
	else if(key<arr[mid])
	BS(arr,i,mid-1,key);
	else
	BS(arr,mid+1,j,key);
	}
}
