# Reconstructing Suspicious Web Activity

## Objective

Use packet-capture evidence to understand how suspicious web activity progressed and which actions were visible in the traffic.

## Method

The report describes filtering HTTP requests by method, source, and URI; reviewing request and response streams; and correlating those observations with TCP conversations. This helped distinguish ordinary page requests from command-bearing requests and relate later web activity to an interactive network session.

## Findings summarized from the lab

The analysis documented a web-form command-injection attempt, subsequent command activity through a web shell, and later page modification. The exact target, addresses, paths, payloads, commands, and timestamps are omitted because they are specific to the provided training capture.

## Tools and techniques

- Wireshark display filters for HTTP requests and TCP conversations
- Follow HTTP Stream and Follow TCP Stream
- Correlation of request times with server responses
- `tshark` for searching across multiple capture files

## Limitations

The PCAP files are not included. This summary does not establish attribution beyond the observations described in the lab report.
