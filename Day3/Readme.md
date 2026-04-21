# Day 3 – OSINT Workflow  
## Infrastructure Intelligence (DNS, IP, Domains & Subdomains)

---

## 1. Objective  

In this task, I performed infrastructure-based OSINT on a target domain. The objective was to understand how a domain is structured and how its underlying infrastructure works.

This includes analyzing DNS records, identifying IP addresses, discovering subdomains, understanding hosting environments, and detecting publicly exposed services. The goal is to map the digital footprint of the organization and understand how it is connected to the internet.

---

## 2. Target  

- **Primary Target:** amrita.edu  

---

## 3. Tools Used  

- WHOIS Lookup (lookup.icann.org)  
- DNSdumpster  
- ViewDNS.info  
- crt.sh  
- BuiltWith  
- Wappalyzer  
- Shodan  

---

## 4. Workflow  

---

## Step 1: Performing WHOIS Lookup  

**Tool I used:**  
lookup.icann.org  

**What I did:**  
I performed a WHOIS lookup to collect basic registration and ownership details of the domain. This is usually the first step in infrastructure intelligence.

**Screenshot:**  
![Step 1](Images/Step1.png)

**What I observed from the screenshot:**  
- The domain name **amrita.edu** is clearly displayed  
- Registrant organization is Amrita Vishwa Vidyapeetham  
- Location details indicate Coimbatore, India  
- Name servers such as `ns1.amrita.edu`, `ns2.amrita.edu` are listed  
- Domain creation and expiry dates are available  
- Administrative and technical contact details are present  

**What I understood:**  
WHOIS provides important background information about the domain, including ownership and management details. It helps identify who controls the domain and whether the information is publicly visible or protected.

---

## Step 2: Analyzing DNS Records  

**Tool I used:**  
DNSdumpster  

**What I did:**  
I entered the domain into DNSdumpster to analyze its DNS records and visualize its infrastructure.

**Screenshots:**  
![Step 2-1](Images/Step2_1.png)  
![Step 2-2](Images/Step2_2.png)  
![Step 2-3](Images/Step2_3.png)  

**What I observed from the screenshots:**  
- A graphical map showing the distribution of servers  
- A Records mapping domains to IP addresses  
- MX Records indicating email servers (linked to Microsoft services)  
- NS Records showing authoritative DNS servers  
- TXT Records containing SPF and verification configurations  
- Multiple subdomains such as `admissions.amrita.edu`, `aaps.amrita.edu`  
- Hosting infrastructure linked to cloud providers and external services  

**What I understood:**  
DNS records act as the backbone of a domain’s infrastructure. This step helped me understand how different services like web hosting, email systems, and DNS management are configured and interconnected.

---

## Step 3: Identifying IP & Hosting Details  

**Tool I used:**  
ViewDNS.info  

**What I did:**  
I used ViewDNS tools to analyze IP-related information such as hosting provider, location, and associated domains.

**Screenshot:**  
![Step 3](Images/Step3.png)

**What I observed:**  
- IP location details such as country and ISP  
- Reverse IP lookup showing other domains hosted on the same server  
- DNS report providing additional configuration details  
- IP history indicating past hosting changes  

**What I understood:**  
This step provides insight into where the domain is hosted and whether it shares infrastructure with other domains. Shared hosting environments can sometimes reveal relationships between different domains.

---

## Step 4: Subdomain Enumeration  

**Tools I used:**  
- crt.sh  
- DNSdumpster  

**Query I used:**  
%.amrita.edu  

**What I did:**  
I searched for all possible subdomains associated with the main domain.

**Screenshot:**  
![Step 4](Images/Step4.png)

**What I observed:**  
- A large number of subdomains were discovered  
- Examples include `admissions.amrita.edu`, `aaps.amrita.edu`, etc.  
- Each subdomain is associated with an IP address  
- Some subdomains may represent internal or specialized services  

**What I understood:**  
Subdomains represent different services or departments within an organization. Identifying them helps in understanding the full attack surface and the number of exposed endpoints.

---

## Step 5: Technology Fingerprinting  

**Tools I used:**  
- BuiltWith  
- Wappalyzer  

**Screenshots:**  
![Step 5](Images/Step5.png)  
![Step 5-1](Images/Step5_1.png)

**What I did:**  
I analyzed the technologies used by the target website.

**What I observed:**  
- Content Management System (CMS): WordPress  
- Backend technologies: PHP  
- Database system: MySQL  
- Email services: Microsoft 365  
- Third-party integrations like analytics tools and media services  

**What I understood:**  
Technology fingerprinting helps identify the software and frameworks used by the website. This information is important for understanding how the system works and for identifying potential vulnerabilities.

---

## Step 6: Shodan Analysis  

**Tool I used:**  
Shodan  

**What I did:**  
I searched for the domain/IP in Shodan to identify publicly exposed services and open ports.

**Screenshot:**  
![Step 6](Images/Step6.png)

**What I observed:**  
- Open ports such as **80 (HTTP)** and **443 (HTTPS)**  
- Server information such as Apache  
- SSL certificate details  
- IP address and geographic location  
- Organization details linked to the domain  

**What I understood:**  
Shodan provides a view of how the domain appears from the internet. It helps identify exposed services and potential entry points, which is important for understanding the security posture of the system.

---

## 5. Conclusion  

In this workflow, I performed a complete infrastructure analysis of the domain using multiple OSINT tools. Starting with WHOIS, I identified ownership details, followed by DNS analysis to understand service configurations.

IP and hosting analysis provided insight into where the system is hosted, while subdomain enumeration revealed additional exposed services. Technology fingerprinting helped identify the software stack, and Shodan analysis highlighted publicly accessible services.

By combining all these steps, I was able to build a comprehensive understanding of the domain’s infrastructure and its presence on the internet.

---

## 6. Practice Note  

For further practice, the same workflow can be applied to:  

- crpf.gov.in  
- Any government or university domain  
- Any publicly accessible organization website  

---
