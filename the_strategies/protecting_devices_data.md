Protecting Your Devices & Stored Data
-------------------------------------

Generally device and data protection is achieved by thoughtfully
combining three techniques: encryption, obfuscation and deletion. Even
in the case of email this triumvirate applies. Encrypt your content with
[GPG](https://www.gnupg.org/), obfuscate your location with the [Tor
Browser Bundle](https://www.torproject.org/projects/torbrowser.html.en),
and securely delete the traces left by your regular activities by using
a disposable operating system like [Tails](https://tails.boum.org/).

> Don’t forget to regularly download, backup and delete your
> email.

### Encrypt Your Devices

Encrypting your various devices is probably the easiest part.
[FileVault](http://support.apple.com/kb/ht4790) comes bundled with Macs,
and [TrueCrypt](https://securityinabox.org/en/truecrypt_main)

> TrueCrypt development ended in May, 2014. [An audit of the
> code is underway](http://istruecryptauditedyet.com/), however, and
> community support may continue.

is free and cross-platform. Both Android devices and iPhones have
built-in encryption options and can be set up in under five minutes.

### Encrypt and/or Obfuscate Groups of Files

Even beyond email, you want to make sure you encrypt and obfuscate
sensitive data stored on your computer, in case you are compelled to
decrypt it. [TrueCrypt](https://securityinabox.org/en/truecrypt_main) is
especially good for this; you can use it to encrypt files on your
computer and then rename the TrueCrypt file to look like something else
entirely, like a movie file. Just make sure that the size of the file
makes sense for the “cover” you give it–a 500 MB .doc file is pretty
unlikely. While similar options don’t currently exist for most phones,
there are research and development efforts in this area.<sup>[48](footnotes/README.html#fn48)</sup> If
you are traveling, consider whether you need to keep sensitive data on
your computer at all. In places with good Internet access, services like
[Martus](https://www.martus.org/index.shtml) can encrypt your files locally and store them
remotely; you don’t even have to keep the key with you if you don’t need
access to them until you get home. Likewise, if your encrypted files are
small enough, you can even transfer them to a USB drive and hide it
somewhere that it’s unlikely to be found in a search.

### Don’t Forget to Delete!

Moving files to the “trash” on your computer–and even “emptying”
it–doesn’t actually do anything to destroy those files; it simply lets
the computer know that the memory they are using can be overwritten if
needed. To really destroy the contents of a file, you need to make sure
it’s overwritten, ideally a few times. Tools like
[CCleaner](http://ccleaner.en.softonic.com/) will let you do exactly that.