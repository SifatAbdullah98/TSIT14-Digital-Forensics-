# Filesystem Forensics

This section summarizes completed partition and filesystem exercises from the lab report. The forensic image and recovered files are not included.

## Exercises

- [Partition analysis](partition-analysis.md): GPT entries and filesystem identification.
- [Inode analysis](inode-analysis.md): ext4 inode location, extraction, and metadata interpretation.
- [Deleted-file analysis](deleted-file-analysis.md): ext4 and NTFS deleted-entry examination, with an unresolved ext4 discrepancy.

## Tools

`mmls`, `fsstat`, `fdisk`, `img_cat`, `blkcat`, `fls`, `icat`, `dd`, `xxd`, `file`, and `istat` are referenced in the report.

## Data handling

The source image, raw inode, recovered images, original paths, and unredacted screenshots are excluded. The NTFS exercise recovered two JPEG files; their contents are not redistributed.
