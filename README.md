# WHUT-AutoHealthReport

通过访问学校健康填报接口，模拟本科生或研究生健康填报过程。并且通过 cqhttp 发送结果到 QQ 号，或通过邮件发送结果到指定邮箱。（支持批量）

配置方法非常简单，第一次运行程序将会进行交互式的配置文件初始化操作，根据提示填写信息后将自动生成配置文件，今后可直接运行程序填报。

程序有 Windows、Linux、macOS 平台的打包版本，无需配置 Python 环境即可运行。

### 效果预览

![Preview](https://assets.zouht.com/img/md/WHUT-AutoHealthReport-README-01.png)

### 使用方法

**运行打包版本**

1. 在右侧 `Releases` 界面下载对应平台版本。
2. 首次运行程序，根据程序提示填写信息。**请注意地址和在校情况的填写，尤其是假期。**
3. 定时运行程序即可自动填报（Linux 可用 `Crontab` 定时执行）

**从源码运行**

1. 确保系统有 `Python3` 环境。
2. 安装模块：`requests`、`PyYAML`
3. 首次运行 `main.py`，根据程序提示填写信息。**请注意地址和在校情况的填写，尤其是假期。**
4. 定时运行 `main.py` 即可自动填报（Linux 可用 `Crontab` 定时执行）

### 免责声明

该自动填报程序仅为了方便每日填报过程，严禁通过该程序伪造填报地址、健康状态。**若使用该程序导致不良后果，使用者需承担所有责任！**

### 问题反馈

如果你使用的时候出现了异常情况，欢迎提交 issue 并附上错误详情，程序日志为同目录的 `log.txt` 文件。

注意，日志中含有敏感隐私信息，不建议直接公开。详细日志中的 `message` 条目和 `Python Traceback` 信息可公开分享。
