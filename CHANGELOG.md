# 变更记录

项目应用中的所有变更记录，将在这个文件中进行存档。

## 目录

* [0.2.5](#025---2022-02-16)
* [0.2.4](#024---2022-02-11)
* [0.2.3](#023---2022-02-08)
* [0.2.1](#021---2022-02-07)
* [0.2.0](#020---2022-01-30)
* [0.1.0](#010---2022-01-27)



## 0.2.5 - 2022-02-16

当前版本调整内容比较多，程序配置文件新增了一些配置项，请留意文档或阅读博客文章。

如果你不希望手动调整程序配置文件，可以在备份当前数据目录 `app` 后，将其中的程序配置文件 `app/config.yml` 删除，重启应用，让程序自动生成新版配置文件。

- [新增] 用户登陆，让公网部署的小伙伴不必担心被陌生人随便修改配置的问题。
- [新增] 免登陆模式，让 HomeLab、本地运行 Flare 的小伙伴，保持使用上的简单。
- [新增] 离线模式，让 Flare 不访问任何公网资源。目前 Flare 仅会调用 issue[#4](https://github.com/soulteary/docker-flare/issues/4) 中提到的 `https://wis.qq.com/weather/common` 接口。
- [新增] 允许用户在页脚自定义展示内容，方便设置诸如个人信息、备案号、用户自己的网站统计脚本等。
- [新增] 允许用户对首页的问候语进行自定义设置，支持设置固定问候语，或根据早晨、中午、下午、晚上几个不同时间段展示不同的内容。
- [优化] 完善应用启动日志输出，方便用户反馈问题。
- [优化] 整理和重构部分代码实现，优化应用渲染性能。

## 0.2.4 - 2022-02-11

解决用户 @ember-zhang 提出的特殊链接渲染和跳转问题，支持了服务端跳转[#3](https://github.com/soulteary/docker-flare/issues/3)。

## 0.2.3 - 2022-02-07

针对应用链接的样式进行调整，让“应用”之间的距离稍微大一些。

修正了用户 @SandZhSand 反馈的在 Firefox 下“应用”书签的一个样式兼容性问题。

## 0.2.1 - 2022-02-07

完善构建脚本，支持在常见的 ARM 设备上直接运行。

## 0.2.0 - 2022-01-30

项目数据存储相关功能重构，使用 yaml 配置进行数据持久化，让应用更加轻量。

## 0.1.0 - 2022-01-27

项目初始化。编写简单的文档，完成基础展示功能，使用 SQLite 进行数据持久化，添加链接图标辅助工具。