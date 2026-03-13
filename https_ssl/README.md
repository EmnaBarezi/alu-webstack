# HTTPS SSL

## Description
This project covers the fundamentals of HTTPS and SSL/TLS encryption,
including how to secure website traffic, configure SSL termination on
HAProxy, and manage domain subdomains.

## Learning Objectives
- Understand the 2 main roles of HTTPS SSL (encryption + authentication)
- Know the purpose of encrypting traffic
- Understand what SSL termination means

## Requirements
- Ubuntu 16.04 LTS
- HAProxy
- Certbot (Let's Encrypt)
- Bash scripts must pass Shellcheck 0.3.7

## Servers
| Name | IP |
|------|----|
| web-01 | 52.90.113.42 |
| web-02 | 44.203.115.14 |
| lb-01 | 18.206.140.94 |

## Tasks

### 0. World Wide Web
Bash script that audits subdomains of a given domain.

**Usage:**
```bash
./0-world_wide_web domain [subdomain]
```

**Example:**
```bash
./0-world_wide_web example.com
./0-world_wide_web example.com web-01
```

## Author
Emna Barezi