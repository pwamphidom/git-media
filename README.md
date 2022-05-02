# Demo Repo Without Git LFS Support

Git-based media demo, without any Git LFS configuration.

**NOTE:** All the files in this repository are uploaded from a browser ("Add file > Upload files") instead of using `git`.

## About this "lfs-not-working" Branch

This branch demonstrates how Git LFS **fails to work for files uploaded through the browser**.

Even if you add `.gitattributes`, the target files will never be indexed (ith LFS pointer) if you upload them with a browser. So when  `git lfs ls-files` command in the terminal, you'll see nothing got indexed.

Files will only be recognized and indexed as "LFS" when you upload with `git push` from your machine.
