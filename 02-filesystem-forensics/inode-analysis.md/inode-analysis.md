# ext4 Inode Analysis

## Objective

Locate and interpret an ext4 inode using filesystem metadata and a raw extraction.

## Method

The report describes using `fsstat` to obtain the filesystem block size, inode size, inodes per group, and inode-table location. Those values were used to calculate the byte offset of inode 48, extract the containing block with `blkcat`, and isolate the inode with `dd`. The raw fields were interpreted according to the ext4 inode layout and checked with `istat`.

The report records the examined inode as 1,249 bytes, owned by numeric UID/GID 1000, with an access time of 2024-07-23 07:16:09 UTC. These are findings from the training image, not general ext4 properties.

## Tools

- The Sleuth Kit: `fsstat`, `blkcat`, `istat`
- Linux utilities: `dd`, `xxd`, `date`
- [Linux ext4 inode documentation](https://www.kernel.org/doc/html/latest/filesystems/ext4/inodes.html)

## Limitations

The raw inode and source image are not included. The calculation is summarized rather than providing a copy of the full lab answer or source-specific extraction paths.
