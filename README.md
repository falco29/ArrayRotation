# ArrayRotation
an interesting code to rotate elements of an array as many places as you want.
#include <math.h>
#include <stdio.h>
#include <string.h>
#include <stdlib.h>
#include <assert.h>
#include <limits.h>
#include <stdbool.h>

int main(){
    int n; 
    printf("enter number of elements of an array:\n");
    scanf("%d",&n);
	int a[20],i,j;
	int temp[10];
	printf("enter array elements:\n");
	for(i=0;i<n;i++){
	scanf("%d",&a[i]);
	}
	int k;
	printf("how many rotations you want?\n");
	scanf("%d",&k);
	for(j=0;j<k;j++){
	
	temp[0]=a[0];
	a[0]=a[n-1];
	for(i=1;i<n;i++){

	temp[i]=a[i];
	a[i]=temp[i-1];
	}}

  
   	for(i=0;i<n;i++){
	printf("%d",a[i]);
	}
	


}
