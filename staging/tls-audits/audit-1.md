## tls-v1-1.badssl.com

SSL Labs grade: B

### Certificate
Status: Valid. The certificate was issued for *.badssl.com by Let's 
Encrypt and OpenSSL returned Verify return code: 0 (ok).

### Protocols
Enabled: TLS 1.1 and TLS 1.2 confirmed through OpenSSL testing.
Deprecated protocols present: Yes, TLS 1.1.

### Ciphers
Weak ciphers present: No major weak cipher was identified during the 
OpenSSL tests. TLS 1.1 negotiated ECDHE-RSA-AES128-SHA, while TLS 1.2 
negotiated ECDHE-RSA-AES128-GCM-SHA256.

### Severity
Rating: Medium

What an attacker could actually do because of this: Supporting TLS 1.1 
allows older and less secure cryptographic protocols to be used. This 
increases the attack surface and may expose users to weaknesses associated 
with outdated TLS implementations.

The specific fix: Disable TLS 1.1 in the web server configuration and 
require TLS 1.2 or TLS 1.3 for all client connections.










