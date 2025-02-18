# 邮件服务器

DCE 5.0 会在用户忘记密码时向用户发送电子邮件以验证他们的电子邮件地址，确保用户是本人操作。要使 DCE 5.0 能够发送电子邮件，您需要像 DCE 5.0 提供您的邮件服务器地址

具体操作步骤如下：

1. 使用具有 `admin` 角色的用户登录 Web 控制台。点击左侧导航栏底部的`全局管理`。

    ![](../../images/ws01.png)

2. 点击`平台设置`，选择`邮件服务器设置`。

    ![](../../images/mail01.png)

    填写以下字段配置邮件服务器：

    - SMTP 服务器地址：能够提供邮件服务的 SMTP 服务器地址。
    - SMTP 服务器端口：端口通常是 `25`。
    - 用户名：SMTP 用户的名称。
    - 密码：SMTP 帐户的密码。
    - 发件人邮箱：发件人的邮箱地址。
    - 使用 SSL 安全连接：SSL 可以用于加密邮件，从而提高通过邮件传输的信息的安全性。通常来说，您必须为邮件服务器配置证书。

3. 配置完成后点击`保存`。

## 常见问题

问：邮件服务器设置后用户仍无法找回密码是什么原因？

答：用户可能未设置邮箱或者设置了错误的邮箱地址；此时可以让有 admin 角色的用户在`全局管理` -> `用户与访问控制`中通过用户名找到该用户，并在用户详情中为该用户设置新的登录密码。

如果邮件服务器没有通，请检查邮件服务器地址、用户名及密码是否正确。
