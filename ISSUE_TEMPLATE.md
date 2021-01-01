Make sure you have provided the following information:

 - [ ] link to your code branch cloned from rhboot/shim-review in the form user/repo@tag
 - [ ] completed README.md file with the necessary information
 - [ ] shim.efi to be signed
 - [ ] public portion of your certificate(s) embedded in shim (the file passed to VENDOR_CERT_FILE)
 - [ ] binaries, for which hashes are added do vendor_db ( if you use vendor_db and have hashes whitelisted )
 - [ ] any extra patches to shim via your own git tree or as files
 - [ ] any extra patches to grub via your own git tree or as files
 - [ ] build logs


###### What organization or people are asking to have this signed:
`Stellar Information Technology Pvt Ltd`

###### What product or service is this for:
`BitRaser Data Eraser Software`

###### What is the origin and full version number of your shim?
`https://github.com/rhboot/shim/archive/15.2.zip`

###### What's the justification that this really does need to be signed for the whole world to be able to boot it:
`Stellar requires to employ secure boot for building trusted operating system. This OS has to be capable of booting every machine so that it can be used with BitRaser Data Eraser software.`

###### How do you manage and protect the keys used in your SHIM?
`Cryptographic USB Token`

###### Do you use EV certificates as embedded certificates in the SHIM?
`Yes`

###### If you use new vendor_db functionality, are any hashes whitelisted, and if yes: for what binaries ?
`[No vendor_db is used]`

###### Is kernel upstream commit 75b0cea7bf307f362057cc778efe89af4c615354 present in your kernel, if you boot chain includes a linux kernel ?
`Yes`

###### if SHIM is loading grub2 bootloader, is CVE CVE-2020-10713 fixed ?
`Yes`

##### Did you change your certificate strategy, so that affected by CVE CVE-2020-10713 grub2 bootloaders can not be verified ?
`This is the first time submission of  SHIM`

###### What is the origin and full version number of your bootloader (GRUB or other)?
`GRUB 2.05 https://github.com/rhboot/grub2/archive/master.zip`

###### If your SHIM launches any other components, please provide further details on what is launched
`SHIM will only launch GRUB. No other component will be launched by the SHIM`

###### How do the launched components prevent execution of unauthenticated code?
`SHIM WILL ONLY LAUNCH SIGNED GRUB AND KERNEL,grub verifies signatures on booted kernels`

###### Does your SHIM load any loaders that support loading unsigned kernels (e.g. GRUB)?
`NO`

###### What kernel are you using? Which patches does it includes to enforce Secure Boot?
`Kernel Version is 5.7.11 it inclued enforce secure boot`

###### What changes were made since your SHIM was last signed?
`This is first time submission`

###### What is the hash of your final SHIM binary?
`SHA512 has is  f6c7c3de781285dfab0a229e118cc736c08c64a823b11e145e272b6b1b90595fe5bc6b1103f91abe6dcf4b09bb91d10ad5029f9e388317bfb355e09282151232`
