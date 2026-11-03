# Deleted-File Analysis

## Objective

Compare deleted-entry examination on ext4 and NTFS and document what the available metadata supports.

## NTFS exercise

The report describes using `fls` with the NTFS partition offset to identify a deleted directory and two deleted JPEG entries. The files were recovered with `icat`, checked with `file`, and opened to confirm that they were readable images. The recovered files and their original names and paths are not included in this repository.

## ext4 exercise: unresolved result

The report states that an ext4 `fls` listing returned three orphan entries: one directory and two regular files. The author reports that running the deleted-entry command produced no output. These accounts conflict, and the discrepancy has not been resolved.

For that reason, this portfolio does not claim that three ext4 orphan entries were independently verified. The report's count should remain an attributed statement until the command, image, partition offset, and run output have been reconciled.

## Tools

- The Sleuth Kit: `fls`, `icat`
- Linux utility: `file`

## Data handling

No disk image, recovered image, original path, or screenshot containing dataset-specific names is included.
