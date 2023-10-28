# 数値リテラル

## C 言語の場合

(他の言語でも同様のルールの場合がある)

```c
#include <stdio.h>

int main(void) {
				printf("%d\n",   10);
				printf("%d\n",  010);
				printf("%d\n", 0x10);
				return 0;
}

```

上記の実行結果

```
10
8
16
```
