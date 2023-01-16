![Release](https://img.shields.io/badge/Release-1.1.0-blue)
---
## 介绍
一款部署在多种平台,基于Python-Flask框架,开发的短网址程序.
## 演示站
[https://url.h2oa.icu](https://url.h2oa.icu)
## 需求
1. 平台: Windows/Linux/Vercel/Netlify.
2. 语言: Python.
3. 包: gunicorn,gevent,flask,flask_cors,pymysql.
4. 数据库: MySql.
## 部署
### 手动
如果需要在Windows/Linux上部署,Windows运行main.py,Linux执行gunicorn main:app -c gunicorn.py.
### 自动
Vecel|Netlify
---|---
[![Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/H2Oa/H2O_Short_Url)|[![Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/H2Oa/H2O_Short_Url)
## 安装
### 手动
首先修改config.py,然后运行/执行
### 自动
1. 首先点击部署的按钮,等待部署完成.
2. 然后添加环境变量,DATABASE_HOST(数据库地址),DATABASE_PORT(数据库端口),DATABASE_USERNAME(数据库用户名),DATABASE_PASSWORD(数据库密码),DATABASE_NAME(数据库名称),DATABASE_PREFIX(数据库前缀,推荐使用h2o_short_url_),DATABASE_SSL_CA_PATH(CA路径),DATABASE_SSL_KEY_PATH(KEY路径),DATABASE_SSL_CERT_PATH(CERT路径),三种证书路径无则空.
![图像1](https://s1.ax1x.com/2023/01/16/pSl2iqK.jpg)
![图像2](https://s1.ax1x.com/2023/01/16/pSl2AaD.jpg)
3. 最后重新部署.
![图像3](https://s1.ax1x.com/2023/01/16/pSl2Pr6.jpg)
![图像4](https://s1.ax1x.com/2023/01/16/pSl2kVO.jpg)
## 配置
1. core表修改网站标题,关键词,描述.
2. domain表修改域名,protocol仅能填http/https.
## 问题
1. 问: Vercel/Netlify自带的域名无法访问.  
   答: Vercel/Netlify自带的域名被DNS污染,需要添加自定义域名.
## 版本
### 1.0
氧化氢短网址程序问世.
### 1.1
1. 增加多种平台的部署.
2. 优化显示.
3. 修改文档.