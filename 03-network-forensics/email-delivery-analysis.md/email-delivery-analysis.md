# Email Delivery Analysis

## Objective

Determine how a suspicious attachment reached a workstation by examining mail-protocol traffic in a packet capture.

## Method

The report describes searching the capture for a distinctive attachment-related string, identifying a POP3 conversation, reviewing the stream and message headers, and decoding the attachment data from the captured transfer.

## Findings summarized from the lab

The report traced a suspicious archive attachment through an email download. It also observed that the mail protocol exposed authentication data in plaintext. All addresses, usernames, passwords, message content, attachment names, hashes, and attachment bytes are omitted.

## Handling note

Do not include a screenshot of the authentication exchange or decoded attachment. Even a screenshot that hides the password can reveal account identifiers, message metadata, and other private details.
