f2fs-backports
==============

The Flash-Friendly File System (f2fs) backported to kernel 3.2 by Now Computing.

This is a patch series to port Samsung's F2FS to kernel 3.2.X.
Currently work is in progress to test and check for correctness. A port to 3.5
kernels is also planned, but it should be mostly a subset of the current patchset
for 3.2 kernels.

This repository is structured as a patchset ready to be merged using "git am".

Instructions for linux 3.2.X kernels:

1. Merge patches found in f2fs_base in order.
2. Merge patches found in f2fs_for_3.2 in order for 3.2 kernels.

Once we have the 3.5 patches ready, we will provide a f2fs_for_3.5 directory.
