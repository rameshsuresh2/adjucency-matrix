#include<stdio.h>
int main() {
  int n1,n2,i,j,o,n,a[10][10];
  printf("Enter the number of connections : ");
  scanf("%d",&n);
  do {
    printf("Enter the matrix : ");
    scanf("%d%d",&n1,n2);
    a[n1][n2]=1;
    a[n2][n1]=1;
    printf("do you want to continue\nif yes press 1\nif no press 0");
    scanf("%d",&o);
  }while(o==1);
  for(i=1;i<=n;i++) {
    for(j=1;j<=n;j++) {
      printf("The matrix is : %d",a[i][j]);
    }
    printf("\n");
  }
  return 0;
}
