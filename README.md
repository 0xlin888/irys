# IRYS领水 -领水比较简单，建议手领，这个脚本主要解决IP不干净，或者IP被占用1拖2、1拖3，领不到的情况
📢 我的推特
🔗[@0x零](https://x.com/0xlin168) 求个关注！如果有任何使用问题，可以通过推特联系我。
## 📌 1. 这个是什么脚本？
这个 Python 脚本用于IRYS领水。

---

## 🛠 2. 需要准备什么？

### ✅ 基础要求
- 一台可以运行 Python 的电脑（Windows / Mac / Linux 都可以）
- 安装 Python（建议使用 Python 3.8 及以上）

### ✅ 安装 Python
如果你的电脑没有 Python，可以按照下面的方式安装：
1. **Windows 用户**：
   - 访问 [Python 官网](https://www.python.org/downloads/) 下载最新版本。
   - 安装时勾选“Add Python to PATH”。
   - 安装完成后，在终端（cmd）输入 `python --version`，如果出现 Python 版本号，说明安装成功。

2. **Mac 用户**：
   - 打开“终端”输入：
     ```sh
     brew install python
     ```
   - 安装完成后，输入 `python3 --version` 检查是否成功。

---

## 📦 3. 安装必需的工具

打开终端（Windows 叫“命令提示符” CMD），输入以下命令安装所需的 Python 库：

```sh
pip install requests openpyxl
```

如果安装成功，你可以输入 `pip list` 来检查它们是否已经安装。

---

## 📊 4. 准备 Excel 文件

在脚本文件夹创建一个 Excel 文件，名称为：wallet.xlsx，文件格式如下：

![](https://raw.githubusercontent.com/0xlin888/irys/refs/heads/main/images/xlsx.png?raw=true)

- **第一列**
- **address**，第一列列名address：IRYS钱包地址
- **第二列**
- **faucet**，第一列列名faucet：不填写，记录领水状态，24小时后再领的时候需要清空状态
---

## 📜 5. 运行脚本

- **5.1 付费打码**

- **修改faucet.py配置**

找到大概第12行，把动态IP API接口换成你自己的
![](https://raw.githubusercontent.com/0xlin888/irys/refs/heads/main/images/nst.png?raw=true)

找到大概第40行，把打码Token换成你自己的

![](https://raw.githubusercontent.com/0xlin888/irys/refs/heads/main/images/no.png?raw=true)

- **5.2 免费打码**
- **也可以本地搭建打码cf-clearance-scraper服务器节省成本**
- 教程参考：https://github.com/0xsongsu/cf-clearance-scraper/
- 使用cf-clearance-scraper用脚本**irys_faucet_cf-clearance-scraper.py**

---

## 🧐 6. 常见问题

### ❓ 如何确认 Python 是否安装正确？
打开终端输入：
```sh
python --version
```
如果出现类似 `Python 3.10.5`，说明安装成功。

### ❓ 运行 `pip install` 时出错？
尝试加 `--upgrade` 重新安装：
```sh
pip install --upgrade requests pandas openpyxl
```
### ❓ 如何运行脚本？

**步骤 1: 打开命令行工具**

Windows**：按 `Win + R`，输入 `cmd`，然后按回车。

Mac/Linux**：打开终端（Terminal）。

**步骤 2: 切换到脚本目录**

使用 `cd` 命令切换到存放 Python 脚本的目录。假设你的脚本在桌面上的 `my_project` 文件夹中，可以使用以下命令：

```bash
cd ~/Desktop/my_project
```
**步步骤 3: 运行脚本**
```bash
python3 script.py
```
script改为你要运行的脚本名
---

## 🛑 7. 免责声明
本脚本仅供学习交流，请自行承担使用风险！使用前请确保了解 OKX 的提现规则。

📌 **有问题？欢迎留言讨论！** 🚀
# irys
