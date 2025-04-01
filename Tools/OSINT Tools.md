# OSINT Tools

---

## Been Verified

**Description:**  
Been Verified is an online people search tool that aggregates public records, social media profiles, and other public data. It produces comprehensive background reports on individuals.

**Use Cases:**

- Conducting background checks
- Gathering contact information and social media profiles
- Verifying identities during investigations

**Details:**

- **Platform:** Web-based
- **Access:** Requires a subscription for detailed reports
- **Usage:** Accessed via its website interface (not available as a CLI tool)

---

## Spokeo

**Description:**  
Spokeo is a people search engine that aggregates data from various online and offline sources. It provides information about individuals, including contact details, social media accounts, and location history.

**Use Cases:**

- Identifying and locating potential subjects
- Gathering social media and contact information
- Verifying personal details for investigative purposes

**Details:**

- **Platform:** Web-based
- **Access:** Subscription-based with various tiers for detailed reports
- **Usage:** Accessed via the Spokeo website interface

---

## ExoneraTor

**Description:**  
ExoneraTor is a service provided by the Tor Project that allows users to determine if a given IP address was a Tor exit node on a specific date.

**Use Cases:**

- Verifying historical use of Tor for anonymizing traffic
- Correlating IP activity with Tor network usage in investigations

**Details:**

- **Platform:** Web-based
- **Usage:** Use the search form by entering the IP address and the date of interest

---

## Whitepages

**Description:**  
Whitepages is a people search tool that aggregates public records to provide contact information, addresses, and background details.

**Use Cases:**

- Locating contact details and residential addresses
- Verifying identities and gathering background data
- Complementing other OSINT methods for a fuller profile

**Details:**

- **Platform:** Web-based
- **Access:** Basic information is free; detailed reports often require payment
- **Usage:** Accessed via the Whitepages website

---

## BuzzSumo

**Description:**  
BuzzSumo is a content intelligence platform that analyzes trending content and identifies key influencers across social media and other online platforms.

**Use Cases:**

- Discovering trending topics and content within a niche
- Identifying influential social media profiles and content creators
- Monitoring content performance and engagement

**Details:**

- **Platform:** Web-based
- **Access:** Subscription-based with various feature levels
- **Usage:** Accessed via the BuzzSumo website

---

## Mention

**Description:**  
Mention is a media monitoring tool that tracks real-time mentions of keywords, brands, or topics across the web and social media.

**Use Cases:**

- Monitoring brand or topic mentions for reputation management
- Tracking emerging trends or potential threats
- Collecting real-time intelligence during investigations

**Details:**

- **Platform:** Web-based
- **Access:** Subscription-based service with configurable alert settings
- **Usage:** Accessed via the Mention dashboard

---

## Factiva

**Description:**  
Factiva is a business information and research tool that aggregates news articles, company profiles, and market research data from a wide range of sources.

**Use Cases:**

- Conducting comprehensive market and business research
- Accessing historical news and data for investigative purposes
- Monitoring industry trends and corporate developments

**Details:**

- **Platform:** Web-based
- **Access:** Subscription-based (commonly used by corporations and research institutions)
- **Usage:** Accessed via the Factiva portal

---

## Sherlock

**Description:**  
Sherlock is a command-line tool used to find usernames across many social networks. It scans over 100 platforms to determine where a given username is registered.

**Use Cases:**

- Discovering a user's digital footprint across multiple platforms
- Correlating online identities during OSINT investigations
- Automating the process of gathering username-based intelligence

| Flag              | Description                                            | Example Usage                                                 |
| ----------------- | ------------------------------------------------------ | ------------------------------------------------------------- |
| `-h`, `--help`    | Display help message and exit                          | `python sherlock.py --help`                                   |
| `-v`, `--verbose` | Enable verbose output for detailed logs                | `python sherlock.py <username> --verbose`                     |
| `-t`, `--timeout` | Set a custom timeout (in seconds) for network requests | `python sherlock.py <username> --timeout 10`                  |
| `-p`, `--proxy`   | Use a specified proxy                                  | `python sherlock.py <username> --proxy http://127.0.0.1:8080` |
| `-o`, `--output`  | Save results to a specified file                       | `python sherlock.py <username> --output results.txt`          |
| `--json`          | Output results in JSON format                          | `python sherlock.py <username> --json`                        |
