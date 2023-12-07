cmake_minimum_required(VERSION 3.15)
project(test)


# 定义变量

# 静态库生成的路径
set(LIBPATH ${PROJECT_SOURCE_DIR}/lib)

# 可执行程序的生成路径
set(EXECPATH ${PROJECT_SOURCE_DIR}/bin)

# 头文件的路径
set(HEADPATH ${PROJECT_SOURCE_DIR}/include)

#库文件的名字
set(CALCLIB calc)
set(SORTLIB sort)

#可执行程序的名字
set(APPNAME1 app1)
set(APPNAME2 app2)

# 给当前节点添加子目录  --添加完子目录，相应的子目录中可以使用这个CMakeLists.txt中定义的变量
add_subdirectory(calc)
add_subdirectory(sort)
add_subdirectory(test1)
add_subdirectory(test2)

