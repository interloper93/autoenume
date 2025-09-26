# AutoEnum

AutoEnum is a reconnaissance and enumeration helper script designed to automate common steps during penetration tests.

## Features (MVP)
- Runs an `nmap` scan with default scripts and service/version detection.
- Parses results and prints open ports + detected services.

## Usage
```bash
python3 autoenum.py <target>

```

## Example
$ python3 autoenum.py 10.10.10.1

[+] Running nmap on 10.10.10.1...

[+] Open Ports Found:
  22/tcp → ssh
  80/tcp → http


---

### Plans for Future Features
- [ ] Run directory brute-forcing (gobuster/ffuf) if HTTP detected  
- [ ] SMB enumeration if port 445 open  
- [ ] Auto-generate Markdown/HTML report  
- [ ] Add multi-target support  
- [ ] Parallel scans for speed    

---

