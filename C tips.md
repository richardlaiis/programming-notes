## 變數

`register` (暫存器變數)，也許可以增加變數存取的效率

```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
int main() {
	register int i, j;
	float sum;
	time_t start, end;
	start = time(NULL);
	for(i = 0; i <= 50000; i++) {
		for(j = 0; j <= 50000; j++) {
			sum += j;
		}
	}
	end = time(NULL);
	printf("execution time: %.3f (s)\n", difftime(end, start));
	return 0;
}
```

## 函式

`inline` 函式，可以將函式的程式嵌入主程式，執行效率增加，但記憶體用量也增加

```c
static inline void input(int n, int x) {
	scanf("%d%d", &n, &x);
	printf("%d\n", (n+x)*(n-x));
}
```
