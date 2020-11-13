## 下载

`Microsoft Store` 搜索`Windows Terminal`，下载并安装

## 配置

```json
{
  // 设置默认打开的终端，此处设置为git bash
  "defaultProfile": "{61c54bbd-c2c6-5271-96e7-009a87ff44b1}",
  "profiles": {
    "defaults": {
      // 此处设置公共属性配置
      "hidden": false
    },
    "list": [
      {
        // git bash.exe
        "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44b1}",
        "name": "Git Bash",
        "commandline": "C:\\Program Files\\Git\\bin\\bash.exe"
      },
      {
        // powershell.exe
        "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
        "name": "Windows PowerShell",
        "commandline": "powershell.exe"
      },
      {
        // cmd.exe
        "guid": "{0caa0dad-35be-5f56-a8ff-afceeeaa6101}",
        "name": "Command Prompt",
        "commandline": "cmd.exe"
      }
    ]
  }
}
```

> 其他配置请自行查阅[配置文档](https://docs.microsoft.com/zh-cn/windows/terminal/)

## 中文乱码问题

```shell
vim C:\\Program Files\\Git\\etc\\bash.bashrc

添加配置
export LANG="zh_CN.UTF-8"
export LC_ALL="zh_CN.UTF-8"
```
