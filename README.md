# CodeAlpha_Snort_IDS
Snort IDS - Detect Ping and Port scan -CODEALPHA TASK 4
cat > README.md << 'EOF'
# Snort Intrusion Detection System - CodeAlpha Task 4

## What I Did
Installed Snort 3 on Kali Linux and configured it as an IDS to detect attacks in real-time.

## Custom Rules (local.rules)
- SID 1000001: CUSTOM - ICMP Ping Detected
- SID 1000002: CUSTOM - SSH Attempt Detected
- SID 1000003: CUSTOM - TCP Scan Detected

## Testing
I ran Snort on eth0 and generated traffic with:
- ping -c 4 8.8.8.8
- nmap -sS 8.8.8.8

## Result
Snort successfully validated the configuration (with 0 warnings).
It detected:
- CUSTOM - ICMP Ping Detected from 10.0.2.15
- CUSTOM - TCP Scan Detected from 10.0.2.15 -> 8.8.8.8

See alerts.txt for proof.

## Tools Used
Kali Linux, Snort 3, Nmap, Ping
EOF
ls -l
