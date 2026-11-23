# dreame-vacuum-blocklist

DNS blocklists for Dreame robot vacuums, built from the DNS queries of a real Dreame L40 Ultra (EU region).
Domain-per-line format, usable in AdGuard Home (Filters, DNS blocklists) and Pi-hole.

| List | Purpose | Risk |
|---|---|---|
| `dreame-vacuum-camera.txt` | Tencent IoT video and STUN (camera / P2P) | Low: live camera view stops |
| `dreame-vacuum-extra.txt` | Other observed hosts, purpose unverified | Higher: test one at a time |

Never block `*.iot.dreame.tech`: it is the control channel.

Raw URLs:

- `https://raw.githubusercontent.com/DavideRutigliano/dreame-vacuum-blocklist/main/dreame-vacuum-camera.txt`
- `https://raw.githubusercontent.com/DavideRutigliano/dreame-vacuum-blocklist/main/dreame-vacuum-extra.txt`

These lists apply to every client that uses the resolver. Hostnames come from one robot and region, so other models or regions may use other names. Not tested on other models. Pull requests welcome.
