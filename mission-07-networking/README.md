# Mission 7 — How Computers Communicate

## Task / Objective

Explain basic networking concepts, test connectivity, look up a domain’s IP addresses, and describe how a browser opens a website.

## Work Completed

### Task 7.1 — Network concepts

| Concept | Explanation | Example |
|---|---|---|
| LAN | Connects devices in a small area, such as a home or office. | My laptop and a printer on the same home network. |
| MAN | Connects networks across a city or metropolitan area. | A city network linking public library branches. |
| WAN | Connects networks across large distances. | A company network connecting offices in different countries. |
| DNS | Looks up information for a domain name, including its IP addresses. | Looking up the IPv4 addresses for `example.com`. |
| Router | Forwards packets between networks. | A home router forwarding traffic to an internet provider. |
| Protocol | A set of rules devices follow to communicate. | HTTPS for secure web communication. |
| Packet switching | Sends data in small packets that can be forwarded independently across a network. | A webpage’s data travels in packets and is reassembled at the destination. |
| Client-server | A client requests something and a server provides a response. | A browser requests a webpage from a web server. |

### Task 7.2 — Connectivity and DNS observations

- `ping -c 4 example.com` sent 4 probes and received 4 replies from `104.20.23.154`. Packet loss was `0.0%`, and the average round-trip time was `25.471 ms`. This showed that the destination answered the probes and measured how long the replies took.
- `dig +short example.com A` returned `104.20.23.154` and `172.66.147.243`. An `A` record lists an IPv4 address for a domain. DNS lets my browser find an address to connect to when I enter a website name.

### Task 7.3 — What happens when I open a website?

1. I enter `https://example.com` in my browser, which acts as the client.
2. The browser needs an IP address for `example.com`. If it has no cached answer, it uses DNS to look one up.
3. My router and other routers forward packets between my computer and the server’s network.
4. The browser establishes a secure connection and requests the page using HTTPS.
5. The server responds with a status code and the page content.
6. The browser interprets the response, requests any additional resources it needs, and displays the page.

## Commands / Tools Used

- `ping -c 4 example.com` checked whether the destination answered four network probes.
- `dig +short example.com A` displayed the domain’s IPv4 addresses.

## My Understanding

DNS tells me which addresses are associated with a website name. Ping tests whether a destination answers network probes. The browser uses HTTPS to request the actual webpage.

## Difficulties Faced

No major difficulties.

## How I Resolved Them

Not applicable.

## Evidence / Files

This README contains the ping statistics and the public IPv4 addresses returned by the DNS lookup.

## Commit Details

- Commit message: `Explain networking concepts and website communication`
-- Push status: Verified on GitHub (commit `04ec10a`).