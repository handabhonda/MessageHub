---

copyright:
  years: 2015, 2017
lastupdated: "2016-11-22"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}


#数据安全和隐私
{: #data_security}


{{site.data.keyword.IBM}} 使用以下方法来帮助确保数据的安全性和隐私性：
{:shortdesc}

## 加密协议
{: #cryptographic notoc}


*  必须使用 TLS 1.2 建立与 Kafka 本机和 REST 接口的连接。
*  连接仅限于以下强密码套件：

      * ECDHE-RSA-AES128-GCM-SHA256
      * ECDHE-RSA-AES256-GCM-SHA384
      * DHE-RSA-AES128-GCM-SHA256
      * kEDH+AESGCM
      * ECDHE-RSA-AES128-SHA256
      * ECDHE-RSA-AES256-SHA384
      * DHE-RSA-AES128-SHA256
      * DHE-RSA-AES256-SHA256



*  要访问 {{site.data.keyword.messagehub}} 仪表板，您必须使用支持 TLS 1.2 的浏览器。
   
## 加密消息有效内容
{: #encryption_payloads notoc}

由于 TLS，会对消息数据进行加密，以便在 {{site.data.keyword.messagehub}} 和客户机之间进行传输。{{site.data.keyword.messagehub}} 会在加密磁盘上存储静态消息数据和消息日志。




