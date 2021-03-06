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


#Seguridad y privacidad de datos
{: #data_security}


{{site.data.keyword.IBM}} utiliza los métodos siguientes para asegurar la
seguridad y privacidad de sus datos:
{:shortdesc}

## Protocolos criptográficos
{: #cryptographic notoc}


*  Las conexiones a Kafka nativo y a las interfaces REST
deben hacerse mediante TLS 1.2. 
*  Las conexiones están restringidas a las siguientes
suites de cifrado fuerte:

      * ECDHE-RSA-AES128-GCM-SHA256 
      * ECDHE-RSA-AES256-GCM-SHA384 
      * DHE-RSA-AES128-GCM-SHA256 
      * kEDH+AESGCM 
      * ECDHE-RSA-AES128-SHA256 
      * ECDHE-RSA-AES256-SHA384 
      * DHE-RSA-AES128-SHA256 
      * DHE-RSA-AES256-SHA256



*  Para acceder al panel de control
de
{{site.data.keyword.messagehub}},
debe utilizar un navegador que admita TLS 1.2. 
   
## Cifrado de la carga útil de mensaje
{: #encryption_payloads notoc}

Los datos de los mensajes se cifran para la
transmisión entre
{{site.data.keyword.messagehub}}
y los clientes como resultado de TLS.
            {{site.data.keyword.messagehub}} almacena datos de mensajes en reposo y registros de mensajes en discos cifrados.




