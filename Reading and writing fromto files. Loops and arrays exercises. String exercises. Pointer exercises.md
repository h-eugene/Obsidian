**Code 1:**
```C
#include <stdio.h>

int fact(int n) {
  int i = 1;
  while (n>0) {
    i*=n;
    n--;
  }
  return (n>=0?i:-1);
}

int check(int n) {
  int sum = 0;
  int i=n;
  while (1<=i) {
    sum+=fact(i%10);
    i/=10;
  }
  return sum==n;
}
int main() {
  int l,r;
  scanf("%d%d",&l,&r);
  for (l;l<r;l++) {
    if (check(l)) printf("%d\n",l);
  }
  return 1;
}
```