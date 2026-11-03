# Evidence Acquisition and Integrity

## Objective

Document the completed forensic imaging and integrity-check workflow without publishing the source evidence or case identifiers.

## Method

The reports describe creating E01 forensic images from source media, then using `ewfverify` to compare the stored acquisition information with a calculated verification result. Analysis was performed from forensic images rather than by changing the original source media.

The lab report also discusses error granularity during acquisition: the block size used when the imaging tool handles read errors affects both acquisition speed and how much nearby data may be treated as bad. The appropriate setting depends on the condition of the source and the risk of losing readable sectors.

## Tools

- `ewfacquire` for E01 acquisition
- `ewfverify` for integrity verification
- `ewfinfo` for image metadata
- MD5 as the hash algorithm recorded in the reports

## Result

The reports state that the verification hashes matched for the acquired images. Image names, hash values, source identifiers, and case-specific details are intentionally omitted from this public summary.

## Evidence handling

- Original media and provided datasets are not included.
- Hashes and image identifiers are not reproduced here.
- The reports describe read-only analysis of acquired images; preserve that distinction when writing about the work.

## Screenshot guidance

The acquisition-verification screenshot in the lab report (page 9, Figure 14) contains image names and hashes. Do not publish it as-is. If sharing is permitted, use a newly captured and redacted output with identifiers and hash values removed.

## Limitations

This repository does not contain the source media or images, so readers cannot independently repeat the acquisition or verify the original hashes.
