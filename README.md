f2fs-backports
==============

The Flash-Friendly File System (f2fs) backported to kernels 3.0 (experimental), 3.2, 3.5 and 3.8 by Now Computing.

This is a patch series to port Samsung's F2FS to previous linux kernel versions.

This repository is structured as a patchset ready to be merged using "git am".

Instructions for linux 3.2.X and 3.5.X kernels:

1. Merge patches found in f2fs-base in order.
2. Merge patches found in f2fs-for-3.5 in order and stop at this step if you want F2FS for 3.5
3. After step 2, merge patches found in f2fs-for-3.2 in order, and you'll have F2FS for 3.2

Instructions for linux 3.8.X kernels:

1. Merge patches found in f2fs-base in order *starting from* patch 78 "f2fs: save device node number into f2fs_inode"
2. Merge patches found in f2fs-for-3.8 in order.

Instructions for linux 3.0.X kernels (should apply to kernels used in recent Android releases):

1. Copy over the patches found in f2fs-for-3.0/f2fs-base to f2fs-base. This will overwrite some patches.
2. Follow instructions for 3.2 kernels.
3. Merge patches found in f2fs-for-3.0 in order.
4. Test it! This version is EXPERIMENTAL and completely untested at the moment.
