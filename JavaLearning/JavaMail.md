# Java电子邮件发送

## 0 纯文本邮件

### 发送一封纯文本邮件需要什么

你需要一些基本的工具来发送一封纯文本的JAVA邮件，我们现在在SpringBoot的语境下讨论这个问题。

- org.springframework.mail.javamail.JavaMailSenderImpl
- org.springframework.mail.javamail.MimeMessageHelper
- javax.mail.internet.InternetAddress
- javax.mail.internet.MimeMessage
- 一个SMTP邮件服务器

#### 可以参考的内容：

1. 首先在项目的配置文件中将邮件服务器的相关配置填写正确，其中主要包括：

   ```yaml
   mail:
     transport:
       protocol: smtp
   	smtp:
   		host: somehost.somedomain.com
   		port: <the port of you host>
   		auth: <whether auth is needed>
   		starttls:
   			enable: true
   		debug: true
   		
   ```

2.  

3. 




## 1 HTML Mail with Template

## 2 MultiPart Mail with MimeMultiPart

