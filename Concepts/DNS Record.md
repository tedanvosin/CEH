# DNS Records

**DNS Record Types** are fundamental for domain management and network troubleshooting. They include:

- **A (Address Record):** Maps a domain to an IPv4 address.
- **AAAA (IPv6 Address Record):** Maps a domain to an IPv6 address.
- **PTR (Pointer Record):** Maps an IP address to a hostname (reverse DNS lookup).
- **SOA (Start of Authority):** Provides administrative information about the domain.
- **CNAME (Canonical Name Record):** Points one domain name to another.
- **MX (Mail Exchange Record):** Specifies the mail servers responsible for receiving email on behalf of the domain.
- **NS (Name Server Record):** Identifies the authoritative name servers for a domain.
- **TXT (Text Record):** Contains arbitrary text data, often used for domain verification and SPF records.
- **HINFO (Host Information Record):** Provides details about the host's hardware and operating system.
- **SRV (Service Record):** Specifies information about available services within the domain.
- **CAA (Certification Authority Authorization):** Indicates which certificate authorities (CAs) are allowed to issue SSL/TLS certificates for the domain.
- **NAPTR (Naming Authority Pointer):** Facilitates dynamic service discovery and is often used in VoIP and other protocols.
- **DS (Delegation Signer):** Used in DNSSEC to authenticate the delegation of a subdomain.
- **DNSKEY:** Contains the public keys used in DNSSEC for verifying DNS records.
- **RRSIG (Resource Record Signature):** Provides a digital signature for a set of DNS records to ensure integrity.
- **NSEC/NSEC3:** Used in DNSSEC to provide authenticated denial of existence, indicating which DNS records do not exist.
