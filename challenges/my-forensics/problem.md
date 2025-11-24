# Stop the exfil

- Namespace: 18739
- Type: custom
- Category: forensics
- Points: 100

## Description

Our organization's SOC saw a burst of odd DNS traffic right before a small web transfer. We suspect
there was a covert file drop but nothing obvious turns up at first glance. We don't have enough time to go through each transfered file. There must be another way. Reconstruct what happened
and recover the flag from the capture.

Download the pcap file: {{url_for("capture.pcap")}}

## Details

You'll need software like wireshark to visualize this file

## Hints

- It would take a long time to check each file sent. What happened before the web traffic?
- What if there was a way to find the correct URL path?
- Are there any DNS queries to a suspicious domain?
- The DNS query names seem to have an interesting format. Why does the word "base32" come to mind?  

## Attributes

- Organization: ACI
- Event: 18739-ctf
