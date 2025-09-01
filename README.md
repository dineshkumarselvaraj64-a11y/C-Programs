# C-Programs
```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main()
{
	 int a, b;
    float x, y;
    scanf("%d %d", &a, &b);
    scanf("%f %f", &x, &y);
    printf("%d %d\n", a + b, a - b);
   printf("%.1f %.1f\n", x + y, x - y);

    return 0;
}
```


```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() 
{
	
    char s[100];
    scanf("%[^\n]%*c", &s);
  	
    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
```


```
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() 
{

    int n;
    scanf("%d", &n);
  	 int size = 2 * n - 1;
     for (int i = 0; i < size; i++) {
        for (int j = 0; j < size; j++) {
             int min_dist = i;
            if (j < min_dist) min_dist = j;
            if (size - 1 - i < min_dist) min_dist = size - 1 - i;
            if (size - 1 - j < min_dist) min_dist = size - 1 - j;

            printf("%d ", n - min_dist);
        }
        printf("\n");
    }
    return 0;
}
````
