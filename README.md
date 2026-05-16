# testingKernelBuilds

Patched Fedora kernel builds for testing purposes; **NOT for production use! ONLY use this if you know exactly what this is!**

The current testing builds are Fedora kernels from the upstream stable kernel 7.0.8, build [kernel-ark](https://gitlab.com/cki-project/kernel-ark)-like by [arkify](https://gitlab.com/knurd42/linux/-/tree/arkify-arkify) to be close to the Fedora kernel.

The builds have two additional patches:

 - PATCHv4 net: skbuff: propagate shared-frag marker through frag-transfer helpers (mitigate a current security issue not contained in 7.0.8 -> like the official Fedora kernel 7.0.8)
 - PATCHv5 v5_flip_done_timeout (the patch this build is intended to test!)

The first patch is to be on par with the Fedora kernel concerning the currenty security issues around Linux distributions: expect that this build's security patches will be obsoleted **likely within a day** due to the current situation around Linux distributions!

As usual with testing builds, retain backups before using this! Also, ensure to be aware of the current security situation when using this a day or more after it had been uploaded, or alternatively, use it only on systems without any security-/privacy-sensitivity!

The builds are provided with the same license as the upstream kernel: GPLv2.
