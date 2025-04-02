# Web/Application Analysis & Data Gathering Tools

---

## Burp Suite

**Description:**  
Burp Suite is an integrated platform for testing web application security. It includes tools such as a proxy, scanner, intruder, and repeater to intercept, inspect, and modify HTTP/HTTPS traffic.

**Use Cases:**

- Intercepting and modifying web traffic
- Automating vulnerability scans
- Performing manual security testing and penetration tests
- Conducting web application audits

**Details:**

- **Platform:** GUI-based (with limited CLI integration for extensions)
- **CLI Flags:** Not applicable

---

## HTTrack WebSite Copier

**Description:**  
HTTrack is a website copier that downloads entire websites for offline analysis, preserving the website’s structure.

**Use Cases:**

- Cloning websites for offline review
- Mapping website structure and content
- Conducting security assessments without interacting with the live site

### HTTrack CLI Flags

| Flag             | Description                                                     |
| ---------------- | --------------------------------------------------------------- |
| `-O <directory>` | Specify the output directory for the copied website.            |
| `-r <depth>`     | Set the maximum recursion depth.                                |
| `-%v`            | Enable verbose mode.                                            |
| `--mirror`       | Enable mirroring (default behavior).                            |
| `-n`             | Restrict download to the specified website (no external links). |

---

## Photon

**Description:**  
Photon is a CLI-based web crawler that extracts information from websites, such as links, images, and email addresses.

**Use Cases:**

- Crawling websites for asset and data extraction
- Collecting metadata and hyperlinks for OSINT investigations
- Gathering web assets for further analysis

### Photon CLI Flags

| Flag            | Description                           |
| --------------- | ------------------------------------- |
| `-u, --url`     | Specify the target URL.               |
| `-o, --output`  | Specify the output directory.         |
| `-d, --depth`   | Set the crawling depth.               |
| `-t, --threads` | Set the number of concurrent threads. |
| `--verbose`     | Enable verbose logging.               |

---

## domianfy.py

**Description:**  
domianfy.py is a CLI tool for gathering domain-related information, including subdomain enumeration, WHOIS data retrieval, and DNS analysis.

**Use Cases:**

- Enumerating subdomains of a target domain
- Gathering WHOIS and DNS information for reconnaissance
- Collecting domain intelligence

### domianfy.py CLI Flags

| Flag            | Description                      |
| --------------- | -------------------------------- |
| `-d, --domain`  | Specify the target domain.       |
| `-o, --output`  | Save output to a specified file. |
| `-v, --verbose` | Enable verbose output.           |

---

## mailfy.py

**Description:**  
mailfy.py is a CLI tool that harvests email addresses from a specified target URL or web pages.

**Use Cases:**

- Extracting email addresses from websites
- Supporting social engineering and OSINT investigations
- Building contact lists for further research

### mailfy.py CLI Flags

| Flag            | Description                                  |
| --------------- | -------------------------------------------- |
| `-u, --url`     | Specify the target URL for email harvesting. |
| `-o, --output`  | Save harvested emails to a specified file.   |
| `-v, --verbose` | Enable verbose output.                       |

---

## searchfy.py

**Description:**  
searchfy.py is a CLI tool designed to automate specialized search queries and aggregate information from web pages.

**Use Cases:**

- Conducting targeted search queries on web data
- Aggregating search results for further analysis
- Automating information retrieval in OSINT investigations

### searchfy.py CLI Flags

| Flag            | Description                              |
| --------------- | ---------------------------------------- |
| `-q, --query`   | Specify the search query.                |
| `-o, --output`  | Save search results to a specified file. |
| `-v, --verbose` | Enable verbose output.                   |

---

## usufy.pf

**Description:**  
usufy.pf is a CLI tool that gathers user-related information, such as social media profiles and online aliases, based on a provided username.

**Use Cases:**

- Searching for social media profiles linked to a username
- Gathering user-specific OSINT data
- Correlating digital identities during reconnaissance

### usufy.pf CLI Flags

| Flag            | Description                       |
| --------------- | --------------------------------- |
| `-u, --user`    | Specify the target username.      |
| `-o, --output`  | Save results to a specified file. |
| `-v, --verbose` | Enable verbose output.            |

---
