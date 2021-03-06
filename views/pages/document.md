# Nice Mail

Nice Mail 是一款以 Markdown 为基础的邮件编辑器。如果你厌倦了平淡无奇的传统邮件格式，那么 Nice Mail 的主题一定能让你眼前一亮。

## 特性

- 支持主题 & 字段配置
- 支持自定义主题
- 支持实时预览
- 支持往编辑器中拖拽上传图片
- 支持 HTML
- 支持 Markdown

## 快速开始

> 如果是第一次使用，请先完成 `发件人配置`。

- 选择主题
- 设置邮件基础信息
- **某些主题可能会有扩展字段，按需填入即可**
- 填写邮件正文（支持拖拽上传图片）
- 发送前可以点击 `预览邮件` 检查一遍
- 最后发送即可

## 发件人字段说明

> 不清楚时，参考各邮件服务商的设置。

| 字段名 | 说明 |
| ------ | ----------- |
| 别名   | 开心就好，方便查看 |
| 发件人邮箱 | 填写发件人邮箱地址，如：`example@example.com` |
| 邮件服务器 | 填写发件人邮箱所对应的服务器地址，如：`smtp.example.com` |
| 用户名 | 填写用户名，一般与发件人邮箱一致即可 |
| 密码 | 对应的密码 |
| TLS | 开启将使用 465 端口 |

**注意：** 如遇填写正确但无法正常使用时请反馈至 [Issue](https://github.com/chuangker/nice-mail/issues)。

## 自定义主题

> 后续完善。

参考项目下 [nice-mail](https://github.com/chuangker/nice-mail/blob/master/templates/nice-mail) 主题模板。

## 常见问题

### 升级后，发件人等信息丢失？

默认情况下，所有的数据都被存放在 Nice Mail 安装的目录下。为了防止升级所造成的数据清空，那么就需要完成以下配置。

```shell
# 获取帮助
$ nice-mail config -h

# 配置缓存数据的目录地址，一般用来缓存发件人等信息
$ nice-mail config --db <dir>

# 配置上传文件的目录地址
$ nice-mail config --upload <dir>
```
