<p align="center">
<a href="https://troubleshooting.tools/lookup/mac/"><img src="https://troubleshooting.tools/assets/img/troubleshooting.tools/gh_logo.png" height="200"></a>
</p>

# DNS Lookup 

DNS Lookup from troubleshooting.tools allows you to query different DNS records for a specific domain. You can retrieve details of different DNS record types such as A, AAAA, CNAME, MX, NS, TXT, SRV, PTR, SOA and more via a Public DNS server of your choice.

## Content
<ol>
<li>) <del>Web page</del></li>
<li>) <del>Webhook</del></li>
<li>) <del>Open Graph</del></li>
<li>) <del>OpenSearch</del></li>
<li>) <del>HTML search form</del></li>
<li>) API</li>
</ol>


## 1.) Web page

coming soon


## 2.) Webhook

coming soon

## 3.) Open Graph

coming soon

## 4.) Open Search

coming soon

## 5.) HTML search form

coming soon

## 6.) API

The DNS Lookup API allows you to query various DNS records for a given domain. You can retrieve details about different DNS record types including A, AAAA, CNAME, MX, NS, TXT, SRV, PTR, SOA, and more via a Public DNS server of your choice. The API supports JSON responses only.

### Features:

* **JSON Response:** Returns detailed information for each queried record type.
* **Support for Multiple Record Types:** You can specify a single record type or query all standard record types in one request.
* **DNS Server Specification:** You can specify a Public DNS server to query. If none is specified, the host will perform the query itself.

### Supported Record Types:
(details provided by [Wikipedia](https://en.wikipedia.org/wiki/List_of_DNS_record_types))

| Type     | Type ID (decimal) | Defining RFC        | Description                                                                                                 | Function                                                                                             |
| -------- | ------------------ | ------------------- | ----------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| A        | 1                  | RFC 1035            | Address record                                                                                             | Returns a 32-bit IPv4 address, commonly used to map hostnames to an IP address.                   |
| AAAA     | 28                 | RFC 3596           | IPv6 address record                                                                                        | Returns a 128-bit IPv6 address.                                                                     |
| AFSDB    | 18                 | RFC 1183            | AFS database record                                                                                         | Location of database servers of an AFS cell.                                                       |
| APL      | 42                 | RFC 3123            | Address Prefix List                                                                                        | Specify lists of address ranges in CIDR format.                                                   |
| CAA      | 257                | RFC 6844            | Certification Authority Authorization                                                                       | Constraining acceptable CAs for a host/domain.                                                     |
| CDNSKEY  | 60                 | RFC 7344            | Child copy of DNSKEY record                                                                                 | For transfer to parent.                                                                              |
| CDS      | 59                 | RFC 7344            | Child DS                                                                                                   | Child copy of DS record, for transfer to parent.                                                   |
| CERT     | 37                 | RFC 4398            | Certificate record                                                                                          | Stores PKIX, SPKI, PGP, etc.                                                                         |
| CNAME    | 5                  | RFC 1035            | Canonical name record                                                                                      | Alias of one name to another.                                                                        |
| CSYNC    | 62                 | RFC 7477            | Child-to-Parent Synchronization                                                                            | Mechanism between a child and a parent DNS zone.                                                   |
| DHCID    | 49                 | RFC 4701            | DHCP identifier                                                                                            | Used with FQDN option to DHCP.                                                                      |
| DLV      | 32769              | RFC 4431            | DNSSEC Lookaside Validation record                                                                          | For publishing DNSSEC trust anchors outside of the DNS delegation chain.                            |
| DNAME    | 39                 | RFC 6672            | Delegation name record                                                                                     | Alias for a name and all its subnames.                                                              |
| DNSKEY   | 48                 | RFC 4034            | DNS Key record                                                                                            | The key record used in DNSSEC.                                                                       |
| DS       | 43                 | RFC 4034            | Delegation signer                                                                                          | Identifies the DNSSEC signing key of a delegated zone.                                             |
| EUI48    | 108                | RFC 7043            | MAC address (EUI-48)                                                                                      | A 48-bit IEEE Extended Unique Identifier.                                                            |
| EUI64    | 109                | RFC 7043            | MAC address (EUI-64)                                                                                      | A 64-bit IEEE Extended Unique Identifier.                                                            |
| HINFO    | 13                 | RFC 8482            | Host Information                                                                                           | Provides minimal-sized responses to DNS queries.                                                    |
| HIP      | 55                 | RFC 8005            | Host Identity Protocol                                                                                     | Separates the end-point identifier and locator roles of IP addresses.                                |
| HTTPS    | 65                 | RFC 9460            | HTTPS Binding                                                                                              | Improves performance for clients resolving many resources.                                          |
| IPSECKEY | 45                 | RFC 4025            | IPsec Key                                                                                                  | Key record that can be used with IPsec.                                                              |
| KEY      | 25                 | RFC 2535/RFC 2930   | Key record                                                                                                 | Used only for SIG(0) and TKEY.                                                                        |
| KX       | 36                 | RFC 2230            | Key Exchanger record                                                                                        | Identifies a key management agent for the associated domain-name.                                   |
| LOC      | 29                 | RFC 1876            | Location record                                                                                            | Specifies a geographical location associated with a domain name.                                     |
| MX       | 15                 | RFC 1035/RFC 7505   | Mail exchange record                                                                                        | List of mail exchange servers that accept email for a domain.                                       |
| NAPTR    | 35                 | RFC 3403            | Naming Authority Pointer                                                                                   | Allows regex-based rewriting of domain names for URIs.                                              |
| NS       | 2                  | RFC 1035            | Name server record                                                                                         | Delegates a DNS zone to use the given authoritative name servers.                                   |
| NSEC     | 47                 | RFC 4034            | Next Secure record                                                                                         | Used to prove a name does not exist.                                                                  |
| NSEC3    | 50                 | RFC 5155            | Next Secure record version 3                                                                                | Allows proof of nonexistence for a name without permitting zone walking.                             |
| NSEC3PARAM| 51                | RFC 5155            | NSEC3 parameters                                                                                           | Parameter record for use with NSEC3.                                                                  |
| OPENPGPKEY| 61                | RFC 7929            | OpenPGP public key record                                                                                  | Publishes OpenPGP public keys in DNS for specific email addresses.                                   |
| PTR      | 12                 | RFC 1035            | PTR Resource Record                                                                                        | Pointer to a canonical name.                                                                          |
| RP       | 17                 | RFC 1183            | Responsible Person                                                                                         | Information about the responsible person(s) for the domain.                                         |
| RRSIG    | 46                 | RFC 4034            | DNSSEC signature                                                                                           | Signature for a DNSSEC-secured record set.                                                            |
| SIG      | 24                 | RFC 2535            | Signature                                                                                                  | Signature record used in SIG(0) and TKEY.                                                            |
| SMIMEA   | 53                 | RFC 8162            | S/MIME cert association                                                                                   | Associates an S/MIME certificate with a domain name.                                                |
| SOA      | 6                  | RFC 1035/RFC 2308   | Start of authority record                                                                                 | Specifies authoritative information about a DNS zone.                                               |
| SRV      | 33                 | RFC 2782            | Service locator                                                                                           | Generalized service location record.                                                                   |
| SSHFP    | 44                 | RFC 4255            | SSH Public Key Fingerprint                                                                                 | Publishes SSH public host key fingerprints in DNS.                                                  |
| SVCB     | 64                 | RFC 9460            | Service Binding                                                                                           | Improves performance for clients resolving many resources.                                          |
| TA       | 32768              | —                   | DNSSEC Trust Authorities                                                                                    | For DNSSEC deployment proposals without a signed DNS root.                                          |
| TKEY     | 249                | RFC 2930            | Transaction Key record                                                                                     | Provides keying material for TSIG that is encrypted under the public key.                             |
| TLSA     | 52                 | RFC 6698            | TLSA certificate association                                                                                | Associates a TLS server certificate with the domain name.                                            |
| TSIG     | 250                | RFC 2845            | Transaction Signature                                                                                     | Authenticates dynamic updates as coming from an approved client.                                      |
| TXT      | 16                 | RFC 1035            | Text record                                                                                               | Originally for arbitrary human-readable text in a DNS record.                                       |
| URI      | 256                | RFC 7553            | Uniform Resource Identifier                                                                                 | Can be used for publishing mappings from hostnames to URIs.                                         |
| ZONEMD   | 63                 | RFC 8976            | Message Digests for DNS Zones                                                                               | Provides a cryptographic message digest over DNS zone data at rest.                                   |

### Input Format:

#### 1. Query by Domain

##### Endpoint:

``` BASH
curl -X GET https://api.troubleshooting.tools/lookup/dns/{domain}/ 
```

##### Example Request:

``` BASH
curl -X GET https://api.troubleshooting.tools/lookup/dns/example.com/ 
```

##### Note:
* If no special record type is specified, the following record types are queried: ```A```, ```AAAA```, ```CNAME```, ```MX```, ```NS```, ```TXT```, ```SRV```, ```PTR```, ```SOA```.

##### Example Response:
``` JSON
{
  "domain": "example.de",
  "dns_server": "localhost",
  "results": {
    "A": [
      "217.160.0.248"
    ],
    "AAAA": [
      "2001:8d8:100f:f000::26f"
    ],
    "CNAME": "No records found for type CNAME.",
    "MX": [
      "10 mx01.ionos.de.",
      "10 mx00.ionos.de."
    ],
    "NS": [
      "ns1078.ui-dns.biz.",
      "ns1078.ui-dns.com.",
      "ns1078.ui-dns.de.",
      "ns1078.ui-dns.org."
    ],
    "TXT": [
      "\"v=spf1 include:_spf-eu.ionos.com ~all\""
    ],
    "SRV": "No records found for type SRV.",
    "PTR": "No records found for type PTR.",
    "SOA": [
      "ns1078.ui-dns.com. hostmaster.1und1.de. 2016041908 28800 7200 604800 300"
    ]
  }
}
```

#### 2. Query by Domain and Record Type

##### Endpoint:

``` BASH
curl -X GET https://api.troubleshooting.tools/lookup/dns/{domain}/{record_type}/
```

##### Example Request:

``` BASH
curl -X GET https://api.troubleshooting.tools/lookup/dns/example.de/A/
```

##### Example Response:

``` JSON
{
  "domain": "example.de",
  "dns_server": "localhost",
  "results": {
    "A": [
      "217.160.0.248"
    ]
  }
}
```

#### 3. Query by Domain and DNS Server

##### Endpoint:

``` BASH
curl -X GET https://api.troubleshooting.tools/lookup/dns/{domain}/{dns_server}/
```

##### Example Request:

``` BASH
curl -X GET https://api.troubleshooting.tools/lookup/dns/example.de/1.1.1.1/
```
##### Note:
* If no special record type is specified, the following record types are queried: ```A```, ```AAAA```, ```CNAME```, ```MX```, ```NS```, ```TXT```, ```SRV```, ```PTR```, ```SOA```.

##### Example Response:

``` JSON
{
  "domain": "example.de",
  "dns_server": "1.1.1.1",
  "results": {
    "A": [
      "217.160.0.248"
    ],
    "AAAA": [
      "2001:8d8:100f:f000::26f"
    ],
    "CNAME": "No records found for type CNAME.",
    "MX": [
      "10 mx00.ionos.de.",
      "10 mx01.ionos.de."
    ],
    "NS": [
      "ns1078.ui-dns.biz.",
      "ns1078.ui-dns.org.",
      "ns1078.ui-dns.de.",
      "ns1078.ui-dns.com."
    ],
    "TXT": [
      "\"v=spf1 include:_spf-eu.ionos.com ~all\""
    ],
    "SRV": "No records found for type SRV.",
    "PTR": "No records found for type PTR.",
    "SOA": [
      "ns1078.ui-dns.com. hostmaster.1und1.de. 2016041908 28800 7200 604800 300"
    ]
  }
}
```

#### 4. Query by Domain, Record Type, and DNS Server

##### Endpoint:

``` BASH
curl -X GET https://api.troubleshooting.tools/lookup/dns/{domain}/{record_type}/{dns_server}/
```

##### Example Request:

``` BASH
curl -X GET https://api.troubleshooting.tools/lookup/dns/example.de/A/1.1.1.1/
```

##### Example Response:

``` JSON
{
  "domain": "example.de",
  "dns_server": "1.1.1.1",
  "results": {
    "A": [
      "217.160.0.248"
    ]
  }
}
```

### Error Handling:
* ```Domain is required```
  * An error message will be triggered if the input domain is missing.

* ```Invalid record type specified```
  * The entered record type is not valid or recognized.

* ```Timeout exceeded for type {record_type}```
  * This error occurs when the DNS server does not respond within the timeout limit.

* ```No records found for type {record_type}```
  * The specified record type is valid, but no matching records were found for the given domain.

* ```HTTP 429: Too Many Requests```
  * Rate limit: 250 requests per second.
  * This limit may be adjusted without prior notice based on server resource demand.

---

All mentioned trademarks are the property of their respective owners.
