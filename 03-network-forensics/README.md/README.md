# Network Forensics

This section summarizes PCAP analysis exercises documented in the lab report. The packet captures, extracted objects, raw payloads, source IP addresses, account details, and case-specific URLs are excluded.

## Exercises

- [Web activity reconstruction](web-activity-reconstruction.md): HTTP requests and streams used to reconstruct suspicious web activity.
- [Download analysis](download-analysis.md): traffic-volume comparison, HTTP object inspection, and protocol analysis.
- [Email delivery analysis](email-delivery-analysis.md): mail-protocol review and attachment handling, with credentials and personal details omitted.

## Tools

Wireshark, `tshark`, and short Python utilities are referenced in the report.

## Handling note

Traffic from a training dataset can contain exploit payloads, account credentials, personal identifiers, and reusable indicators. Those details are not reproduced here. The summaries focus on the investigation steps and the evidence types used.
