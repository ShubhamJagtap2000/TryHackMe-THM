# What happens when you make a DNS request?

## 1. 

When you request a domain name, your computer first checks its local cache to see if you've previously looked up the address recently; 

if not, a request to your **Recursive DNS Server** will be made.

## 2.

A Recursive DNS Server is usually provided by your ***ISP**, but you can also choose your own. 

This server also has a **local cache** of recently looked up domain names. 

If a result is found locally, this is sent back to your computer, and your request ends here. 
(this is common for popular and heavily requested services such as Google, Facebook, Twitter)

If the request cannot be found locally, a journey begins to find the correct answer, starting with the internet's **root DNS servers**.

## 3.

The **root servers** act as the DNS backbone of the internet; their job is to `redirect` you to the correct `Top Level Domain Server`, depending on your request. For example,

You request www.tryhackme.com, the root server will recognise the Top Level Domain of `.com` and refer you to the correct `TLD server` that deals with `.com` addresses.

## 4.

The `TLD server` holds records for where to find the **authoritative server** to answer the DNS request. 

The authoritative server is often also known as the `nameserver` for the domain. For example,

The nameserver for `tryhackme.com` is `kip.ns.cloudflare.com` and `uma.ns.cloudflare.com`. 

You'll often find multiple **nameservers** for a domain name to act as a backup in case one goes down.

## 5.

An **authoritative DNS server** is the server that is responsible for storing the DNS records for a particular domain name and where any updates to your domain name DNS records would be made. 

Depending on the record type, the DNS record is then sent back to the **Recursive DNS Server**, where a local copy will be cached for future requests and then relayed back to the original client that made the request. 

DNS records all come with a `TTL (Time To Live)` value. 

This value is a number represented in seconds that the response should be saved for locally until you have to look it up again. 

`Caching` saves on having to make a DNS request every time you communicate with a server.

   
   ![Screenshot (744)](https://user-images.githubusercontent.com/63872951/178140378-d8938e72-96ad-42ed-8bbb-aee99f133f5f.png)



# Answer the questions below

1.  What field specifies how long a DNS record should be cached for?
```
TTL
```
2.  What type of DNS Server is usually provided by your ISP?
```
Recursive
```
3.  What type of server holds all the records for a domain?
```
Authoritative
```





