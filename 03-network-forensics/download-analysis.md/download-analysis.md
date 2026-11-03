# Download and Protocol Analysis

## Objective

Examine network conversations and downloaded objects to assess suspicious delivery activity.

## Method

The lab report describes using Wireshark conversation statistics to prioritize large transfers, resolving names from DNS responses present in the capture, reviewing HTTP requests and responses, exporting HTTP objects, and checking file types independently of their declared content type. It also compares stream bytes with expected protocol headers when a connection on a familiar port does not appear to use the expected protocol.

## Findings summarized from the lab

The report identified downloaded objects whose actual file type did not match the server's declared image type. It also described a large encoded response and a separate binary protocol carried over a port commonly associated with HTTPS. The report assessed these as suspicious; the raw files and case-specific indicators are not included.

## Tools and techniques

- Wireshark conversations, protocol hierarchy, and stream inspection
- HTTP object export
- `tshark` DNS lookups against capture data
- Python for joining and decompressing response chunks
- `file` for file-type identification

## Limitations

No packet capture, extracted object, malware sample, hash, domain, or IP address is distributed. A file-type mismatch is an investigative lead and should be corroborated before calling a file malicious.
