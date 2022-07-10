# Domain Hierarchy

   ![Screenshot (743)](https://user-images.githubusercontent.com/63872951/178138845-dac55ad7-577f-42af-9389-b4eee1119dfb.png)

   
## TLD (Top-Level Domain)

- A TLD is the **most righthand part** of a domain name. 

So, for example, the tryhackme.com TLD is .com. 

- There are two types of `TLD`, `gTLD (Generic Top Level)` and `ccTLD (Country Code Top Level Domain)`. 

- Historically a gTLD was meant to tell the user the domain name's purpose; for example, 

  - **.com** would be for commercial purposes, 
  - **.org** for an organisation, 
  - **.edu** for education and .gov for government. 
  - **ccTLD** was used for geographical purposes, for example, **.ca** for sites based in Canada, **.co.uk** for sites based in the United Kingdom and so on. 

Due to such demand, there is an influx of new **gTLDs** ranging from **.online** , .club , .website , .biz and so many more. 

For a full list of over **2000** TLDs [click here](https://data.iana.org/TLD/tlds-alpha-by-domain.txt).

## Second-Level Domain

- Taking `tryhackme.com` as an example, the **.com** part is the **TLD**, and `tryhackme` is the `Second Level Domain`. 

- When registering a domain name, the second-level domain is limited to `63 characters + the TLD` and can only use `a-z 0-9` and **hyphens**. 

(cannot start or end with hyphens or have consecutive hyphens)

## Subdomain

- A subdomain sits on the `left-hand side` of the **Second-Level Domain** using a period to separate it; 
 
- for example, in the name `admin.tryhackme.com` the `admin` part is the `subdomain`. 
 
- A subdomain name has the same creation restrictions as a Second-Level Domain, being limited to `63 characters and can only use a-z 0-9` and **hyphens**. 
 
(cannot start or end with hyphens or have consecutive hyphens). 

- You can use multiple subdomains split with periods to create longer names, such as `jupiter.servers.tryhackme.com`. 
- But the length of the `domain name` must be kept to `253 characters or less`. 
- There is `no limit` to the number of subdomains you can create for your domain name.

# Answer the questions below

1.  What is the maximum length of a subdomain?
```
63
```
2.  Which of the following characters cannot be used in a subdomain ( 3 b _ - )?
```
_
```
3.  What is the maximum length of a domain name?
```
253
```
4.  What type of TLD is .co.uk?
```
ccTLD
```







