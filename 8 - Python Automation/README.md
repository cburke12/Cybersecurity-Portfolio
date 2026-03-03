# Module 8 - Python Security Automation

## Objective
Write Python scripts to automate common security tasks: log parsing, file integrity checking, alert generation, and security tool integration. Apply PEP 8 standards and write clean, well-documented code.

## Skills Demonstrated
- Python Programming (PEP 8)
- Log File Parsing & Analysis
- File I/O Operations
- String Manipulation & Regular Expressions
- Security Automation Scripting
- Hash-based File Integrity Verification
- Brute-force Detection via Sliding Window Logic

## Tools Used
- Python 3
- VS Code / Cursor
- Linux CLI
- GitHub

## Projects
- **8.1 - Log Parser:** Extract and count failed SSH login attempts from auth logs *(in progress)*
- **8.2 - File Integrity Checker:** Compare SHA-256 hashes of files to detect tampering *(in progress)*
- **8.3 - Brute-Force Detector:** Sliding-window script to flag IPs exceeding login failure threshold *(in progress)*
- **8.4 - Automated Alert Script:** Parse logs and output structured JSON alerts for suspicious activity *(in progress)*
- **8.5 - Port Scanner (basic):** Python socket-based scanner to identify open ports on a target host *(planned)*

## Sample Script Snippet
```python
import re
from collections import defaultdict

def parse_failed_logins(log_file):
    """Extract IPs with failed SSH login attempts."""
    pattern = r'Failed password for .+ from (\d+\.\d+\.\d+\.\d+)'
    counts = defaultdict(int)
    with open(log_file, 'r') as f:
        for line in f:
            match = re.search(pattern, line)
            if match:
                counts[match.group(1)] += 1
    return dict(sorted(counts.items(), key=lambda x: x[1], reverse=True))
```

## Status
> In progress. Python scripts being written as part of Security+ prep and home lab work. All projects in this module are written in Python 3.
