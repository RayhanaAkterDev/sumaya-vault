---
class: cse
title: 03 Discuss the main divisions of the domain name space.
course:
  - Computer Network
chapter:
  - Chapter 7 - Application Layer
semester: 6th
date: 2025-09-10
status: pending 🛑
importance: ⭐⭐⭐
tags:
  - board_2019
---
# Main Divisions of the Domain Name Space

The **Domain Name Space** is the hierarchical structure used by the Domain Name System (DNS) to organize and manage domain names on the internet. It is arranged like an inverted tree, with the **root domain** at the top and all other domains branching out below it. This structure ensures global uniqueness, efficient management, and scalability of internet addressing.

---

## Main Divisions of the Domain Name Space

1. **Root Domain**  
    The root domain is the highest level in the hierarchy and is represented by a dot ("."). Although users do not usually type it, it serves as the starting point for all domain name lookups. The root contains pointers to all top-level domains and is managed by a set of root name servers distributed worldwide.
    
2. **Top-Level Domains (TLDs)**  
    Directly below the root domain are the Top-Level Domains. These are the first-level divisions of the internet namespace. TLDs are further categorized into:
    
    - **Generic TLDs (gTLDs):** Common domains such as _.com, .org, .net, .info_.        
    - **Sponsored TLDs (sTLDs):** Domains sponsored by specific organizations, like _.edu, .gov, .mil, .aero_.        
    - **Country Code TLDs (ccTLDs):** Two-letter domains representing countries, like _.bd_ (Bangladesh), _.uk_ (United Kingdom), _.jp_ (Japan).
        
3. **Second-Level Domains**  
    These domains appear directly to the left of a TLD and are usually chosen by organizations or individuals to represent their names or brands. For example, in _example.com_, “example” is the second-level domain. They are often used to identify specific organizations, businesses, or projects under a TLD.
    
4. **Third-Level Domains (Subdomains)**  
    Third-level domains, also called **subdomains**, are subdivisions of second-level domains. They are often used to organize content or services within a website. For instance, _mail.google.com_ or _blog.example.org_. Subdomains allow flexibility and logical structuring of services.
    
5. **Hostnames**  
    At the lowest level, hostnames identify individual devices or services within a domain. For example, _server1.department.university.edu_ is a hostname that points to a specific machine within the university’s network. Hostnames represent the leaf nodes of the domain name space tree.