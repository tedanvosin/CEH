# Password Cracking & Authentication Exploits Tools

---

## Cain & Abel

**Description:**  
Cain & Abel is a Windows-based password recovery tool that uses techniques such as network sniffing, dictionary attacks, brute-force attacks, and cryptanalysis to recover passwords from various sources.

**Use Cases:**

- Recovering passwords from network traffic
- Cracking hashed passwords stored on a system
- Performing Windows password audits

**Details:**

- **Platform:** Windows (GUI-based)
- **CLI Flags:** Not applicable

---

## John the Ripper

**Description:**  
John the Ripper is an open-source password cracking tool designed to identify weak passwords. It supports multiple hash types and employs various attack methods such as dictionary, brute-force, and hybrid attacks.

**Use Cases:**

- Cracking Unix/Linux password hashes
- Auditing password strength
- Recovering forgotten or weak passwords during penetration tests

**Details:**

- **Platform:** CLI-based (available on Windows, Linux, and macOS)

### John the Ripper CLI Flags

| Flag                       | Description                                                  |
| -------------------------- | ------------------------------------------------------------ |
| `--wordlist=<file>`        | Specify a wordlist file for dictionary attacks.              |
| `--rules`                  | Enable additional word mangling rules for the attack.        |
| `--format=<format>`        | Specify the hash format (e.g., MD5, DES, etc.).              |
| `--fork=<n>`               | Split the workload across _n_ processes.                     |
| `--incremental[=<mode>]`   | Use incremental (brute-force) mode; optionally specify mode. |
| `--session=<name>`         | Save or resume a session with the given name.                |
| `--status`                 | Display the current status of the cracking process.          |
| `--show`                   | Display cracked passwords.                                   |
| `--restore`                | Restore a previously saved session.                          |
| `--pot=<file>`             | Specify a custom pot file to store cracked passwords.        |
| `--max-run-time=<seconds>` | Set the maximum run time for the cracking process.           |

---

## hashcat

**Description:**  
hashcat is a GPU-accelerated password recovery tool that supports a wide range of hash algorithms and attack modes. It is known for its speed and efficiency in cracking high-complexity passwords.

**Use Cases:**

- Cracking high-complexity password hashes using GPU power
- Performing large-scale password audits
- Evaluating password strength and security in vulnerability assessments

**Details:**

- **Platform:** CLI-based (available on Windows, Linux, and macOS)

### hashcat CLI Flags

| Flag                       | Description                                                |
| -------------------------- | ---------------------------------------------------------- |
| `-m <num>`                 | Specify the hash mode (e.g., 0 for MD5, 100 for SHA1).     |
| `-a <num>`                 | Set the attack mode (0 = straight, 3 = brute-force, etc.). |
| `-o <file>`                | Write found passwords to the specified file.               |
| `--outfile-format <num>`   | Specify the output file format.                            |
| `-w <num>`                 | Set the workload profile (1 to 4).                         |
| `--status`                 | Enable periodic status display.                            |
| `--status-timer <seconds>` | Set the interval for status display updates.               |
| `-O`                       | Enable optimized kernel (may limit password length).       |
| `--quiet`                  | Suppress output.                                           |
| `-S`                       | Show only the cracked passwords.                           |
| `--session <name>`         | Name the session for resume purposes.                      |
| `--restore`                | Restore a session from a restore file.                     |
| `--benchmark`              | Run benchmark tests.                                       |
| `--help`                   | Display help message and exit.                             |

---

## L0phtCrack

**Description:**  
L0phtCrack is a password auditing and recovery tool for Windows that evaluates password strength, recovers passwords from hashes, and performs brute-force or dictionary attacks.

**Use Cases:**

- Auditing password security in Windows environments
- Recovering weak or forgotten passwords
- Assessing password policies and compliance

**Details:**

- **Platform:** Windows (GUI-based)
- **CLI Flags:** Not applicable

---
