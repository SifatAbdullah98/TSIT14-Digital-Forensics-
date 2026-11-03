# Windows Memory Forensics

## Scope

This section summarizes the Windows memory-analysis exercises in the lab report (pages 36–59). The memory image, extracted files, credential material, host identifiers, and unredacted screenshots are not included.

## Analysis areas

- Identifying the operating-system build and locating registry hives
- Reviewing system and network configuration artifacts
- Examining process lists, services, and memory scan results
- Correlating event-log evidence with process and service activity
- Reviewing user activity artifacts such as UserAssist, browser history, and recent documents
- Recording clock anomalies and incomplete or unavailable artifacts as limitations

## Tools

Volatility 2 and Volatility 3 are referenced in the report, along with event-log extraction and small scripts for filtering records. Public plugin names used for non-credential analysis include `windows.info`, `windows.registry.hivelist`, `windows.registry.printkey`, `windows.pstree`, `windows.psscan`, `windows.netscan`, `windows.svcscan`, and `windows.registry.userassist`.

## Findings summarized from the lab

The report correlated suspicious service and process activity with event logs and network artifacts. It also documented limitations, including a system clock that was corrected during operation and commands that could not be recovered from memory. No passwords, hashes, account names, system names, addresses, malware filenames, or file hashes are reproduced here.

## Limitations

The memory image and extracted artifacts are not distributed, so these observations cannot be independently repeated from this repository.
