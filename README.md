# INLIGHNX-TECH-INTERN-OFF-CYB-SEC---PORT-SCANNER

A simple Python port scanner used to scan a range of ports on a target host or IP address. Useful as a learning project for basic networking and security tooling.

## Features
- Scan single host or a range of ports
- TCP connect-based scanning (fast, reliable)
- Command-line interface with options for host, port range, and timeout
- Cross-platform (requires Python 3.8+)

## Requirements
- Python 3.8 or newer
- (Optional) virtualenv / venv for isolated environment

## Installation
Clone the repo and install dependencies (if any):
```bash
git clone https://github.com/NavinAdithya/INLIGHNX-TECH-INTERN-OFF-CYB-SEC---PORT-SCANNER.git
cd INLIGHNX-TECH-INTERN-OFF-CYB-SEC---PORT-SCANNER
# create a venv (recommended)
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
.\.venv\Scripts\activate    # Windows PowerShell
# If there is a requirements.txt:
pip install -r requirements.txt
```

## Quickstart / Usage
Run the scanner with required arguments. Examples assume the scanner script is named `scanner.py` — replace with actual filename if different.

Scan a single host on common ports:
```bash
python scanner.py --host example.com --ports 20-1024
```

Scan a single port:
```bash
python scanner.py --host 192.168.1.10 --port 22
```

Example flags:
- `--host` or `-t` : target hostname or IP
- `--port` or `-p` : single port (e.g., 80)
- `--ports`       : port range (e.g., 1-1024)
- `--timeout`     : socket timeout in seconds
- `--threads`     : number of worker threads (if supported)

If the project provides a script entrypoint, you can also run:
```bash
python -m port_scanner --host 1.2.3.4 --ports 1-1024
```

## Output
The scanner prints open ports to stdout and may optionally write results to a file if the script supports it.

## Security & Usage Notes
- Use this tool only on hosts you own or have explicit permission to test.
- Port scanning can trigger IDS/IPS or be considered hostile activity on third-party networks.

## Tests
If test files exist, run:
```bash
pytest
```
or the command indicated by the repo.

## Contributing
Contributions and bug reports welcome. Open an issue or a PR with a clear description and reproduction steps.

## License
No license file detected. Recommended: MIT. Reply if you want me to add an MIT LICENSE file automatically.

## Maintainer
Maintained by https://github.com/NavinAdithya
