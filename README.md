# hotupdate
C++热更新方案

1、主要逻辑在 main.cpp 文件里面的信号处理函数 sig_user1_handler 里面

2、使用nm命令查找C++编译后的函数名

3、编译 make server so

4、main为主程序，so 为热更文件

5、先用./main 运行程序，然后使用 kill -SIGUSR1 `pidof main` 命令查看运行结果


