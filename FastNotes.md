## Notes:

### Target Scan

```bash
# get open port & serves
curl https://search.censys.io/hosts/{ip}| grep "<h2" | cut -d '"' -f2

# get TCP only
curl https://search.censys.io/hosts/{ip} | grep "<h2" | cut -d '"' -f2 | grep "TCP"

# sub domain scan 
curl https://sonar.omnisint.io/subdomains/{Host} 

#Phone search
curl https://search.illicit.services/records?phoneNumbers={PhoneNumber}

#Email search
curl https://search.illicit.services/records?emails={Email}

#usernames search
curl https://search.illicit.services/records?usernames={UserName}
```
