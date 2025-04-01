# Network Scanning and Mapping Tools

---

## hping (hping3)

Description:
hping is a command-line oriented packet crafting and network scanning tool.
It can be used for advanced network scanning, firewall testing, and network debugging.

Use Cases:

- Crafting custom TCP/IP packets to test network responses.
- Performing advanced network scans and diagnostics.
- Evaluating firewall rules and detecting packet filtering.

Usage Example:
hping3 -S -p 80 <target_IP>

| Flags             | Details                                                          |
| ----------------- | ---------------------------------------------------------------- |
| -S                | Set the SYN flag.                                                |
| -A                | Set the ACK flag.                                                |
| -F                | Set the FIN flag.                                                |
| -R                | Set the RST flag.                                                |
| -P                | Set the PSH flag.                                                |
| -U                | Set the URG flag.                                                |
| -s <port>         | Set the source port (e.g., -s 53).                               |
| -p <port>         | Set the destination port (e.g., -p 80).                          |
| -c <count>        | Number of packets to send.                                       |
| -i <interval>     | Interval between packets (e.g., -i u1000 for 1000 microseconds). |
| -d <data_size>    | Specify packet payload size.                                     |
| -E <file>         | Use file as packet payload.                                      |
| --icmp            | Use ICMP protocol instead of TCP/UDP.                            |
| --udp             | Use UDP protocol.                                                |
| --tcp             | Force TCP mode.                                                  |
| -n                | Numeric output only (no DNS resolution).                         |
| -V                | Print version information.                                       |
| -v                | Increase verbosity level.                                        |
| -q                | Quiet mode (minimal output).                                     |
| -a <address>      | Specify a spoofed source address.                                |
| -w <window>       | Set TCP window size.                                             |
| -M <seq>          | Set initial sequence number.                                     |
| --rand-source     | Use a random source IP address.                                  |
| --ttl <value>     | Set IP Time To Live.                                             |
| --frag            | Set IP fragmentation flag.                                       |
| --ipproto <proto> | Specify the IP protocol number.                                  |
| --help            | Display help message and exit.                                   |

---

## Fing

Description:
Fing is a network scanning tool that identifies devices on a local network.
It detects connected devices, lists their IP addresses, and provides vendor information.

Use Cases:

- Identifying all devices connected to a network.
- Troubleshooting network connectivity issues.
- Creating a network inventory for security assessments.

Usage Example:
fing 192.168.1.0/24

| Flags           | Details                                  |
| --------------- | ---------------------------------------- |
| -h, --help      | Display help information.                |
| -v, --version   | Display version information.             |
| -o, --output    | Specify output format (e.g., JSON, CSV). |
| -q, --quiet     | Minimal output.                          |
| -r, --resolve   | Perform DNS resolution on found IPs.     |
| --timeout <sec> | Set scan timeout duration.               |
| --ports <range> | Specify a port range to scan.            |
| --verbose       | Enable verbose output.                   |

(Note: Fing's available flags may vary by version; please refer to the Fing documentation for the full list.)

---

## Nmap

Description:
Nmap (Network Mapper) is an open-source tool for network exploration and security auditing.
It supports host discovery, port scanning, service detection, OS detection, and more.

Use Cases:

- Discovering hosts on a network.
- Scanning for open ports and identifying running services.
- Performing vulnerability assessments and security audits.

Usage Example:
nmap -A <target_IP_or_network>

| Flags                     | Details                                                                                          |
| ------------------------- | ------------------------------------------------------------------------------------------------ |
| -sS                       | Perform a SYN (stealth) scan.                                                                    |
| -sT                       | Perform a TCP connect scan.                                                                      |
| -sU                       | Perform a UDP scan.                                                                              |
| -sV                       | Probe open ports to determine service/version info.                                              |
| -O                        | Enable OS detection.                                                                             |
| -A                        | Aggressive scan mode (enables OS detection, version detection, script scanning, and traceroute). |
| -p <ports>                | Specify target port(s) (e.g., -p 1-65535).                                                       |
| -T<0-5>                   | Set timing template (e.g., -T4 for faster execution).                                            |
| --script <scripts>        | Run specified Nmap Scripting Engine (NSE) scripts.                                               |
| -v, -vv                   | Increase verbosity level.                                                                        |
| -d, -dd                   | Increase debugging level.                                                                        |
| --open                    | Show only open (responding) ports.                                                               |
| --reason                  | Display the reason a port is in a particular state.                                              |
| --packet-trace            | Show all packets sent and received.                                                              |
| --traceroute              | Perform traceroute to the target.                                                                |
| --version-all             | Try every single probe for version detection.                                                    |
| --disable-arp-ping        | Disable ARP ping (useful in some local network scans).                                           |
| --max-retries <num>       | Set the maximum number of probe retransmissions.                                                 |
| --host-timeout <time>     | Set a maximum time allowed for scanning a host.                                                  |
| --min-rate <number>       | Specify minimum packet send rate.                                                                |
| --max-rate <number>       | Specify maximum packet send rate.                                                                |
| --resume <file>           | Resume a previously aborted scan from a file.                                                    |
| --iflist                  | List available interfaces and routes.                                                            |
| --datadir <directory>     | Specify a custom data directory.                                                                 |
| --script-args <n1=v1,...> | Pass arguments to NSE scripts.                                                                   |
| --stats-every <sec>       | Print scan statistics every specified seconds.                                                   |
| --append-output           | Append to an existing output file.                                                               |
| --unprivileged            | Assume non-root user (limits scan types).                                                        |
| --privileged              | Force privileged mode.                                                                           |
| --help                    | Display help message and exit.                                                                   |

(Refer to Nmap's official documentation for an exhaustive list of options.)

---

## Maltego

Description:
Maltego is a data mining and visualization tool that maps relationships between entities (people, websites, domains, etc.).
It is used for comprehensive link analysis and threat intelligence.

Use Cases:

- Visualizing network infrastructures and data relationships.
- Mapping digital footprints during investigations.
- Integrating and analyzing data from multiple sources.

Usage:
Maltego is a GUI-based application. Users interact with it via its visual interface.
No command-line flags are available.

---

## Gephi

Description:
Gephi is an open-source network visualization and analysis tool.
It is used for graphing and analyzing large network datasets.

Use Cases:

- Visualizing complex network structures.
- Analyzing clusters and connectivity in network data.
- Academic research and professional network analysis.

Usage:
Gephi is a desktop GUI-based application. Users load network data and apply visualization algorithms via the interface.

---

## NodeXL

Description:
NodeXL is an Excel-based network analysis and visualization tool.
It integrates with Microsoft Excel to help users create and analyze network graphs.

Use Cases:

- Creating network graphs and visualizations within Excel.
- Analyzing social networks and data connectivity.
- Simplifying network analysis for users familiar with Excel.

Usage:
NodeXL is used as an add-in within Microsoft Excel.
No command-line flags are available.

---
