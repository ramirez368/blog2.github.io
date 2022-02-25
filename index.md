---
layout: default
---

[How Emails Works](https://www.youtube.com/watch?v=x28ciavQ4mI).

[//]: #  There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Steps and Explanation of the E-mail Process and Protocols.
We all use emails because it is fast and makes our lives easier.  In the conventional mailing system, the processing time was indefinite. When comparing both systems, there is a drastic difference. However, in some unusual situations, the emails could be delayed unpredictably.

Knowing how the email system works is important to all the email users. However, most of us are unaware of what goes on behind the scenes. Learning this will help to figure out the status of your emails sent that ended up in an error or with a bounce back message.

We will see the working of emails in detail in this article.

 

## What is email?

The term “email” stands for “electronic mail”. The electronic mail is introduced first in the 1960s, however it became available in the current structure in the 1970s. Let us take a look at how email actually works.

 

## Protocols used in email systems

The email communication is done via three protocols in general. They are listed below.

IMAP
POP
SMTP
 

## IMAP

The IMAP stands for Internet Mail Access Protocol. This protocol is used while receiving an email. When one uses IMAP, the emails will be present in the server and not get downloaded to the user’s mail box and deleted from the server. This helps to have less memory used in the local computer and server memory is increased.

## POP

The POP stands for Post Office Protocol. This protocol is also used for incoming emails. The main difference with the both protocols is that POP downloads the entire email into the local computer and deletes the data on the server once it is downloaded. This is helpful in a server with less free memory. Current version of POP is POP3.

## SMTP

The SMTP stands for Simple Mail Transfer Protocol. Email is sent using this protocol.

 



The diagram down below describes the path that email takes from your computer to the intended recipient . This shows the path of the email from sending to receiving ends. There are also many logical machines in the email delivery process. Please have a look at the diagram before proceeding

[![How does email work?](https://www.interserver.net/tips/wp-content/uploads/2016/08/Email-Working.png)

## Mail Server

A mail server is a computer application. This application receives incoming emails from the local users (people within same domain) as well as remote senders and forwards outgoing email for delivery. A computer having such an application installed can also be called as a mail server. Here, this is the case of what we call a mail server. Here, in the diagram you can see two mail servers. The two mail servers which are used for outgoing emails are called as MTAs, mail transfer agents. The other two mail servers used for incoming, using POP3/IMAP protocols are called as MDAs, the mail delivery agents.

 

## DNS

The DNS stands for Domain Name System. The purpose of the DNS is to translate the domain names to the IP addresses and vice-versa. The DNS is used here to find out the mail server of the other side. This information is retrieved from the DNS and the email message is sent to the particular email address.

 

## How Emails Work

First the sender needs to enter the email address of the recipient along with the message using an email application. This should be done at the local computers. Once it is finished and the “Send” button is clicked, the email will be going to the MTA (The Mail Transfer Agent). This communication is done via the SMTP protocol.

The next step is DNS lookup. The system sends a request to find out the corresponding MTA of the recipient. This will be done with the help of the MX record. In the DNS zone, for the receiver address’ domain, there will be an MX record (stands for Mail Exchanger record). This is a DNS resource record which specifies the mail server of a domain. So, after the DNS lookup, a response is given to the requested mail server with the IP address of the recipient’s mail server. This way the ‘to’ mail server is identified.

The next step is transferring the message between the mail servers. The SMTP protocol is used for this communication. Now our message is with the recipient mail server (MTA).

Now, this message is transferred to the Mail Delivery Agent and then it is transferred to the recipient’s local computer. As we have seen earlier, two protocols can be used here. If we use POP3, then the whole email will be downloaded to the local computer and the copy at the server gets deleted. If the protocol used is IMAP, then the email message is stored in the mail server itself, but the user can easily manipulate the emails on the mail server as in the local computer. This is the difference when using both the protocols and this is how your email gets delivered. If some error occurred to send the email, the emails will be delayed. There is a mail queue in every mail server. These mails will be pending in the mail queue. The mail server will keep trying to resend the email. Once the email sending fails permanently, the mail server may send a bounce back email message to the sender’s email address.

This explains why you maybe getting bounce back emails sometimes. The reason for bouncing back will be explained in the message. There are many reasons for getting an email to bounce back such as as incorrect email address in the ‘to’ field


```
Thank you readers, and wait for Blog 3 next week.
For Contact e-mail me at ramirez368@hotmail.com

```
