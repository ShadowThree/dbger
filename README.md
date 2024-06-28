## 简介
1. 本项目是简单的嵌入式日志输出管理模块；
2. 可以通过`MCU Uart`或者是`JLink RTT`输出日志；
3. 可以配置日志输出级别；

## 使用说明
1. 通过`git submodule add https://github.com/ShadowThree/dbger.git ThirdUtils/dbger`添加本项目到工程指定目录；
2. 配置`dbger.h`；
3. 在`main.c`中调用：
```c
#include "dbger.h"

int main(void)
{
    // ...
    LOG_INIT();
    LOG_DBG("dbger test\n");
    // ...
}
```