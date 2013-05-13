f2fs-backports
==============

The Flash-Friendly File System (f2fs) backported to kernels 3.2 and 3.5 by Now Computing.

This is a patch series to port Samsung's F2FS to kernel 3.2.X and 3.5.X.

This repository is structured as a patchset ready to be merged using "git am".

Instructions for linux 3.2.X kernels:

1. Merge patches found in f2fs-base in order.
2. Merge patches found in f2fs-for-3.5 in order and stop at this step if you want F2FS for 3.5
3. After step 2, merge patches found in f2fs-for-3.2 in order, and you'll have F2FS for 3.2

Linux 3.8 patches soon!
