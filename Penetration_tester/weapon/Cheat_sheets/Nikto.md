# Nikto

Nikto is a powerful assessment tools for finding vulnerabilities in web servers.

# Scanning a host

Nikto -h <Hostname/IP>

# Scanning specific ports

Nikto -h <Hostname/IP> -port <Port Number>,<Port Number>

# Maximum scan time

Nikto -h <Hostname/IP> -maxtime <Number in Seconds>

# Scanning duration

Nikto -h <Hostname/IP> -until

# Disable SSL

Nikto -h <Hostname/IP> -nossl

# Force SSL

Nikto -h <Hostname/IP> -ssl

# Disable 404 guessing

Nikto -h <Hostname/IP> -no404

# Ignore negative responses. 302,301

Nikto -h <Hostname/IP> -IgnoreCode <Code Number>

# Update the plugins and databases

Nikto -update

# Specify host header

Nikto -h <Hostname/IP> -vhost

# Output results

Nikto -h  <Hostname/IP> -output <filename>

# Scanning through a proxy

Nikto -h <Hostname/IP> -useproxy <Proxy IP>

# Host authentication

Nikto -h <Hostname/IP> -id id:pass or id:pass:realm

# Database check

Nikto -h <Hostname/IP> -dbcheck

# Config file

Nikto -h <Hostname/IP> -config <nikto.conf>

# Disable name lookups on IP addresses

Nikto -h <Hostname/IP> -nolookup

# Disable response cache

Nikto -h <Hostname/IP> -nocache

# Disable interactive features

Nikto -h <Hostname/IP> -nointeractive

# Display options

Nikto -h <Hostname/IP> -Display <Option>
1 Show redirects
2 Show Cookies
3 Show 200/OK responses
4 Show URL requiring authentication
D Show debug output
E HTTP Errors
P Print progress to STDOUT
S Scrub output of IP and Hostname
V Verbose output

# Evasion Options

Nikto -h <Hostname/IP> -evasion <Option>
1 Random URI Encoding
2 Directory Self-Reference /./
3 Premature URL ending
4 Prepend long random string
5 Fake parameter
6 TAB as request spacer
7 Change the case of the URL
8 Used windows directory separator \
A Use a carriage return (0x0d) as a request spacer
B  Use binary value (0x0b) as a request spacer

# Output File Format

Nikto -h <Hostname/IP> -Format <Option>
csv       Comma-separated-value
htm    HTML Format
msf+  Log to Metaspoloit
nbe     Nessus NBE
txt       Plain text
xml    XML Format

# Tuning

Nikto -h <Hostname/IP> -Tuning <Option>
1   Interesting file
2   Misconfiguration
3   Information Disclosure
4   Injection (XSS/Script/HTML)
5   Remote File Retrieval – Inside Web Root
6   Denial of Service
7   Remote File Retrieval – Server Wide
8   Command Execution – Remote Shell
9   SQL Injection
0   File Upload
a   Authentication Bypass
b   Software Identification
c   Remote Source Inclusion
x   Reverse Tuning Option

# Mutate

Nikto -h <Hostname/IP> -mutate <Option>
1   Test all files in root directory
2   Guess for password file names
3   Enumerate user names via apache
4   Enumerate user names via cgiwrap
5   Attempt to brute force sub-domain names
6   Attempt to guess directory names from a file.