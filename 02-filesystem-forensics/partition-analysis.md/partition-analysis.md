# GPT Partition and Filesystem Analysis

## Objective

Identify the partition layout of a forensic disk image and determine the filesystem type of each relevant partition.

## Method

The lab report documents this sequence:

1. Use `mmls` to inspect the disk layout and locate partition boundaries.
2. Examine the GPT partition entries to interpret their type identifiers.
3. Cross-check the partition information with `fdisk`.
4. Use `fsstat` with the relevant partition offset to identify filesystem metadata.

## Tools

- The Sleuth Kit: `mmls`, `fsstat`, `img_cat`
- Linux utilities: `fdisk`, `dd`, `xxd`

## Result

The examined image contained two primary data partitions, one using ext4 and one using NTFS. The partition layout was cross-checked with more than one tool. Dataset-specific offsets, sector ranges, image names, and raw partition-table bytes are omitted.

## Limitations

The source image is not distributed, so the result cannot be independently reproduced from this repository.
