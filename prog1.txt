#include <stdio.h>
int main(){
    int a,i;
    printf("enter size:");
    scanf("%d",&a);

    int arr[a];
    printf("enter elements:\n");
    for(i=0;i<a;i++)
        scanf("%d",&arr[i]);

    int l=arr[0],s=arr[0];

    for(i=1;i<a;i++){
        if(arr[i]>l)
            l=arr[i];
        if(arr[i]< s)
            s=arr[i];
    }
    printf("largest = %d\n smallest = %d",l,s);
    return 0;
}
