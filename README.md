# new & delete

strcpy & strcpy_s

```C++
#define _CRT_SECURE_NO_WARNINGS
#include <iostream>
#include <cstring>

char* MakeStrAdr(int len)
{
  char* str = (char*)malloc(sizeof(char) * len);
  
  return str;
}

int main()
{
  char* str = MakeStrAdr(20);
  strcpy(str, "I am so happy~");
  
  std::cout<< str <<std::endl;
 
  free(str);
 
  return 0;
}
```
