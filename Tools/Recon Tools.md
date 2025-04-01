# Recon Tools
---

## theHarvester

Description:
theHarvester is a command-line tool that gathers emails, subdomains, hostnames, and virtual hosts from public sources like search engines, PGP key servers, and SHODAN.

Use Cases:

- Enumerate email addresses and domain information.
- Identify subdomains and hostnames for further investigation.
- Collect data to support phishing or social engineering campaigns.

Basic Usage:
```
theHarvester -d example.com -l 100 -b google
```

| Flags | Description                          |
| ----- | ------------------------------------ |
| -d    | Specify the target domain            |
| -l    | Limit the number of results          |
| -b    | Choose the data source               |
| -f    | Save output to a file in HTML format |
| -h    | Display help information             |

---

## Recon-ng

Description:
Recon-ng is an interactive reconnaissance framework offering a modular environment to integrate multiple data sources and automate information gathering tasks.

Use Cases:

- Aggregate data from various sources in one framework.
- Automate repetitive reconnaissance tasks.
- Analyze target data to identify vulnerabilities.

Details:

- Platform: CLI-based interactive framework.
- Usage: Launch the tool by typing "recon-ng" in the terminal. Within its interactive shell, load modules and run commands.

Example Commands:
``` 
  recon-ng> workspaces add mytarget
  recon-ng> modules load recon/domains-hosts/google_site
  recon-ng> run
```
---

## Spyse

Description:
Spyse is a comprehensive reconnaissance platform that aggregates technical data about domains, IP addresses, and digital assets. It offers insights into network infrastructure and potential vulnerabilities.

Use Cases:

- Map target network infrastructures.
- Identify associated digital assets and vulnerabilities.
- Integrate with automated scripts via API access.

Details:

- Platform: Web-based with API support.
- Usage: Access via the Spyse web interface or use its API (refer to Spyse documentation for API details).

---
