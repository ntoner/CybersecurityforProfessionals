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


## incomplete-chain.badssl.com

SSL Labs grade: B

### Certificate

Status: Certificate chain is incomplete. SSL Labs identified a missing 
intermediate certificate, which causes certificate-chain validation issues for 
some clients.

### Protocols

Enabled: TLS 1.0 and TLS 1.1 are supported. TLS 1.3 is not supported. 
Deprecated protocols present: Yes.

### Ciphers

SSL Labs did not identify a separate cipher-strength issue in the summary. The 
primary issue for this host is the incomplete certificate chain and support for 
deprecated TLS versions.

### Severity

Rating: Medium

What an attacker could actually do because of this: An incomplete certificate 
chain can cause clients to be unable to fully validate the server's 
certificate. This can lead to trust and connectivity problems and may cause 
users or applications to accept weaker validation behavior.

The specific fix: Install and correctly configure the missing intermediate 
certificate so the server presents the complete certificate chain. TLS 1.0 and 
TLS 1.1 should also be disabled and TLS 1.2 or TLS 1.3 should be required.

---

## dh480.badssl.com

SSL Labs grade: F

### Certificate

Status: The SSL Labs scan completed successfully. The primary security issue 
identified was the use of insecure Diffie-Hellman key exchange parameters.

### Protocols

Enabled: TLS 1.0 and TLS 1.1 are supported. TLS 1.3 is not supported. 
Deprecated protocols present: Yes.

### Key Exchange

Weak Diffie-Hellman parameters present: Yes. SSL Labs identified insecure DH 
key exchange parameters associated with the Logjam vulnerability. The audit 
also identified a 480-bit Diffie-Hellman configuration.

### Severity

Rating: High

What an attacker could actually do because of this: Weak Diffie-Hellman 
parameters reduce the strength of the key exchange and can make cryptographic 
protections significantly easier to attack. This can increase the risk of an 
attacker weakening the confidentiality of encrypted communications.

The specific fix: Replace the 480-bit Diffie-Hellman parameters with 
appropriately sized modern parameters and disable weak DH configurations. TLS 
1.0 and TLS 1.1 should also be disabled and TLS 1.2 or TLS 1.3 should be 
required.







