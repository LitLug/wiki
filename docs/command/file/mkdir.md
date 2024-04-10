# mkdir 命令 – 新建目录

## 命令详解

```bash
mkdir [-p] path
```

来自英文词组 `make directory` 的缩写，其功能是新建一个目录。

| 参数 | 注释                                 |
| ---- | ------------------------------------ |
| -p   | 确保路径中的所有路径存在，如无则创建 |

## 实例

!!! example "范例 1"

    执行以下命令可以在当前目录新建一个名为 `MyFolder` 的文件夹。
    ```bash
    [lug@litwiki ~]# mkdir ./MyFolder
    ```

!!! example "范例 2"

    执行以下命令可以在当前目录新建一个名为 `Folder1` 的文件夹，并在其中新建一个名为 `MyFolder` 的文件夹

    :fontawesome-solid-circle-xmark:{: .orangered } **错误**格式：
    ```bash
    [lug@litwiki ~]# mkdir ./Folder1/MyFolder
    ```
    因为 `Folder1` 目录不存在，无法执行并报错

    :fontawesome-solid-circle-check:{: .limegreen } **正确**格式：
    ```bash
    [lug@litwiki ~]# mkdir -p ./Folder1/MyFolder
    ```
    此时若 `Folder1` 不存在，将会新建 `Folder1` 后再在其中新建 `MyFolder` 目录
