## func Remove(name string) error

参数列表

- name 文件或目录名

返回值：

- 返回error 返回错误信息对象

功能说明：

这个函数主要是删除一个文件或目录

代码实例：

    package main

    import (
        "fmt"
        "os"
    )

    func main() {
        err := os.Remove("Hello.go")
        if err != nil {
            fmt.Printf("Error: %s\n", err)
            return
        }
        fmt.Printf("Hello.go has been removed!\n")
    }

代码输出：

    //test in ArchLinux
    Hello.go has been removed!
