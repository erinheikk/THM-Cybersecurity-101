# Search Skills and OSINT Tools
Quick reference notes THM Cyber101 Search Skills

## Shodan (TryScanMe)
Search engine for IoT but also used for discovering internet-connected devices
### Query Filters
country: restrict results to a specific country code (ex. Country:IE)

port: filter by a specific port number or range (ex. Port:22)

org: scope results in a named organization or ASN Identifier (Who owns a range of IP addresses) (ex. AS7224 which is Amazon Web Services)

hostname: match against a specific hostname or domain (ex. hostname:fakebank.thm)

## VirusTotal (TryDetectMe)
VirusTotal collates results from over 70 antivirus engines and website scanners into a single interface. Submit a file, a URL, a domain, or a file hash. VirusTotal will tell you whether any of those engines have flagged it as malicious or not.

While not foolproof, VirusTotal is a popular resource in the blue teaming community for obtaining a general consensus on suspicious files and links, as well as for gathering intelligence on new threats on the move.

## NIST Common Vulnerabilities and Exposures (CVE)
Universal dictionary of known vulnerabilities

Each confirmed vulnerability is assigned a unique identifier in the format CVE-YEAR-NUMBER, such as CVE-2025-55182. If the vulnerability is impactful enough, it may even get a moniker (ex. vulnerabilities such as Heartbleed, React2Shell, and Log4Shell). These vulnerabilities are given a score (CVSS) based on a variety of factors, such as:

Impact - What damage can this vulnerability lead to?

Complexity - Is the vulnerability easy to exploit or not?

Availability - How likely is it that someone can exploit this?

## LINUX MAN (Manual) Pages
These pages serve as documentation that you can read within your terminal about any command on Linux, and a majority of cybersecurity tooling

To view the manual page, run: man <command>

## GitHub
Researchers often publish proof-of-concept (PoC) code, exploitation tools, and detailed technical reports there, which are usually faster than official channels

Searching for a CVE identifier (e.g., CVE-2026-1337) directly on GitHub often reveals repositories containing PoC code, scanner scripts, or detailed analyses of the vulnerability.

That said, not all PoCs are equally reliable. Some are incomplete, some are intentionally flawed, and occasionally a "PoC" repository is malicious itself. Always verify what you're about to execute.
