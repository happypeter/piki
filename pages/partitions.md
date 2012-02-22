---
layout: page
title: Partitions
---

 know that you are only allowed 4 primary partitions, that the extended
partition holds the logical partitions, that you can have unlimited logical
partitions in your one extended partition, and that the extended partition is
a primary partition.

So my questions are the following:

1. Why does the computer make the distinction? What about the way the computer
   reads the drive requires there to be only 4 primary partitions? Why can't
there be unlimited primary partitions?

2. Does a primary partition have unique functionality that a logical partition
   doesn't (other than being able to be an extended partition).

3. Will having a primary partition rather than logical partition lead to
   slightly faster access times because of the way the computer looks each up?
Will it matter on the scale of personal computer?

Thanks for your time!


1. Because DOS was rubbish, blame Microsoft. It's a legacy thing, and is long
   long irrelevant in terms of the limitations of modern computers, however
without a replacement partitioning scheme e.g GPT -
http://en.wikipedia.org/wiki/GUID_Partition_Table you're stuck with it.

Wellll ...
2). Some BIOS manufacturers were as brain-dead as M$oft, and required
"bootable" partitions to be primary. *And* you had one (only one) marked as
bootable.
And yes, that applied even if you only had Linux on the box.

How lame.

Edit: Windows requires primary partitions for certain purposes, including
booting Windows. This is a Windows design limitation; Linux can boot just fine
from a logical partition.

http://en.wikipedia.org/wiki/Disk_partitioning
