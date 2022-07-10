# DNS Record Types

`Domain Name System (DNS)` is the protocol responsible for resolving hostnames, such as **tryhackme.com**, to their respective IP addresses. 

DNS isn't just for websites though, and multiple types of DNS record exist. 

We'll go over some of the most common ones.

## A Record

These records resolve to `IPv4 addresses`, for example `104.26.10.229`

## AAAA Record

These records resolve to `IPv6 addresses`, for example `2606:4700:20::681a:be5`

## CNAME Record

These records resolve to another domain name, for example, 

TryHackMe's online shop has the `subdomain` name ***store.tryhackme.com*** which returns a CNAME record ***`shops.shopify.com`***. 

Another DNS request would then be made to ***shops.shopify.com*** to work out the IP address.

## MX Record

These records resolve to the address of the servers that handle the email for the domain you are querying, for example,

An `MX record` response for ***tryhackme.com*** would look something like ***`alt1.aspmx.l.google.com`***. 

These records also come with a `priority flag`. 

This tells the client in which order to try the servers, this is perfect for if the main server goes down and email needs to be sent to a backup server.

## TXT Record

`TXT` records are `free text fields where any text-based data can be stored`. 

TXT records have multiple uses, but some common ones can be to **list servers that have the authority to send an email on behalf of the domain** (this can help in the battle against `spam` and `spoofed email`).

They can also be used **to verify ownership of the domain name when signing up for third party services**.

# Answer the questions below

1.  What type of record would be used to advise where to send email?
```
MX
```
2.  What type of record handles IPv6 addresses?
```
AAAA
```
