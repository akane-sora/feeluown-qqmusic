# feeluown QQ 音乐插件

[![Build Status](https://travis-ci.com/feeluown/feeluown-qqmusic.svg?branch=master)](https://travis-ci.com/feeluown/feeluown-qqmusic)
[![PyPI](https://img.shields.io/pypi/v/fuo_qqmusic.svg)](https://pypi.python.org/pypi/fuo-qqmusic)
[![Coverage Status](https://coveralls.io/repos/github/feeluown/feeluown-qqmusic/badge.svg?branch=master)](https://coveralls.io/github/feeluown/feeluown-qqmusic?branch=master)

## 安装

```sh
pip3 install fuo-qqmusic
```

## 使用说明

### 登录
在网页登录微信/QQ后（在任意网站），复制请求中的 cookies 至程序登录框

Step by Step Guide:

1.打开 qq 音乐网站

2.登录

3.在网页上鼠标右键，点击「检查元素」（英文叫 Inspec）。或者直接按 F12。就会看到类似这样的窗口
![Inspec](https://user-images.githubusercontent.com/4962134/94247236-6cbc4b00-ff4f-11ea-94b2-c64ff5679ec0.png)

4.点击「网络」（英文叫 Network）
![Network](https://user-images.githubusercontent.com/4962134/94247417-ad1bc900-ff4f-11ea-87df-518c74f35513.png)

5.拷贝 cookies，复制到 feeluown 的登录窗口

## changelog

### 0.3 (2020-08-10)

感谢 [@csy19960309](https://github.com/csy19960309)

- 支持登陆功能，加载用户歌单
- 支持歌词和 mv
- 绿钻用户可以播放任意歌曲，但不能选音质

### 0.2 (2019-11-27)
- 使用 marshmallow>=3.0

### 0.1.5 (2019-10-28)
- 支持获取歌手的所有歌曲与专辑

### 0.1.4 (2019-08-20)
- 修复获取部分歌曲链接失败

### 0.1.3 (2019-05-25)
- 给歌曲链接添加过期时间

### 0.1.2 (2019-03-27)
- 获取音乐链接时，先尝试 M500 品质的，再尝试使用网页版接口返回的
  (测试发现：部分歌曲网页版接口拿不到链接，所以修改策略)

### 0.1.1 (2019-03-19)
- 获取音乐链接时，使用和网页一样的接口

### 0.1 (2019-03-18)
- 简单的搜索功能，歌曲、歌手、专辑详情查看
