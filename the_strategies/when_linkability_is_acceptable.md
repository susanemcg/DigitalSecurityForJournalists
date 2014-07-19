When Linkability is Acceptable
------------------------------

In the bulk of day-to-day journalism, source linkability is not a
paramount concern. We tend to prefer our sources “on the record” in the
first place, and once quoted in an article their connection to us is
public–and published–knowledge.

At the same time, concision isn’t the only reason we don’t publish
entire interview transcripts. Most source conversations contain a mix of
“on” and “off the record” remarks; not everything we discover in an
interview should be discoverable. Yet if these exchanges take place
through (unencrypted) email, shared documents, or chat applications,
“discoverable”–both legally and technically–is exactly what they are.

As in the physical world, no digital security measure is absolute, and
ultimately the onus falls on individual journalist or organization to
determine which measures should be baseline and which applied only in
certain cases. Whatever the decision, however, its consequences will
most substantially be borne by your source, not yourself. A situation
need not be life-threatening to be a significant risk: Loss of a job or
professional standing, family and marital consequences, financial and/or
legal liabilities can all be the fallout of source communications coming
to light. In the majority of cases, the risk you take is not your own.

> “We’re allowed to make choices about risks to ourselves, not our
> sources.”\
> –Jonathan Stray

### Encrypt to Protect

The main key to protecting your communications with known sources is
simple: Encrypt, encrypt, encrypt.<sup>[43](footnotes/README.html#fn43)</sup> Where encryption isn’t
possible for legal, technical, or resource reasons, consider
communication alternatives that may be more familiar to your
correspondents or have better legal protections, such as postal mail.

No matter the communication method, there is a good range of solutions
out there for all kinds of devices. Android devices tend to have a
greater variety of open-source options, but there are several trusted
cryptographers making solutions for Apple devices as well. In general,
authentication and encryption require that both parties use the
particular app in question; this can made Web-based solutions like
[CryptoCat](https://crypto.cat/) valuable for journalists trying to move
their sources to more secure communications channels, since only a
browser plug-in is required.<sup>[44](footnotes/README.html#fn44)</sup>

### **Web Browsing**

If you’ve ever worked in a large organization, chances are you’ve had to
use a “virtual private network,” or VPN at one point or another. VPNs
funnel all of your Web traffic through an encrypted tunnel into the
network for which they are configured. This provides two types of
protection for Web activity, in that it both encrypts your traffic and
obfuscates its origin, by sending it first to your organization’s
network–wherever in the world that is–and *then* out to the broader
Internet, no matter where you are. Using your company VPN or a similar
commercial solution like [Private Internet
Access](https://www.privateInternetaccess.com/) or
[TorGuard](http://torguard.net/) to route your Web traffic through a
known network can help protect you from a potentially hostile Web
provider.<sup>[45](footnotes/README.html#fn45)</sup> Keep in mind, however, that while the ISP you’re
on will only know that you’re using a VPN, your company or VPN provider
will be able to see all of the Web requests you make. An IPsec VPN will
route not just your browser traffic but all of your Web traffic (e.g.
for applications like DropBox etc.) through the VPN.

To truly *anonymize* the location of your Web browsing activity,
however, the [Tor Browser
Bundle](https://www.torproject.org/projects/torbrowser.html.en) is your
best bet. The Tor Browser is an open-source, cross-platform browser,
described in more detail below, that is an important tool for
anonymizing your location online, especially in places where VPNs may be
banned outright.

### **Email**

Email [presents a special security problem for a number of
reasons](http://www.forbes.com/sites/kashmirhill/2013/08/09/lavabits-ladar-levison-if-you-knew-what-i-know-about-email-you-might-not-use-it/),
but the first step you can take is not to store your emails on any Web
server longer than necessary. Set up a local email application like the
free, open-source and cross-platform
[Thunderbird](https://www.mozilla.org/en-US/thunderbird/) on your
computer and connect it to your regular email account. Even if you don’t
use the application much on a day-to-day basis, you can use it to follow
a “download-and-delete” protocol where every three months or so, you
download all of your emails that are more than a few months old and
archive them locally. After you’ve backed them up to an external hard
drive, delete the copies on your Web-based email provider. You will
still be able to save and search your old emails, but since they reside
on your own physical computer, they will be better protected against
subpoena-based searches.

Thunderbird also provides support for encrypting and authenticating
email, through its
[Enigmail](https://addons.mozilla.org/en-US/thunderbird/addon/enigmail/?src=search)
add-on and [GPG](https://www.gnupg.org/).

> GPG ([GnuPrivacy Guard](https://www.gnupg.org/)) is the
> open-source version of PGP (“Pretty Good Privacy”), which was created
> by Phil Zimmerman.

While setting up some of these systems can take several steps, once
you’ve generated your public-private key pair

> For more information on working with GPG, see the [GPG Mini How
> To](http://www.dewinter.com/gnupg_howto/english/GPGMiniHowto.html)

and connected it to your email application, all of this happens in the
background. The software can store the public keys of your
correspondents, and performs the necessary encryption/decryption and
signing of your messages with the click of a button. Though Google
recently announced [an “end-to-end” encryption option for
Gmail](http://googleonlinesecurity.blogspot.com/2014/06/making-end-to-end-encryption-easier-to.html),
the fact that it’s still decrypted in the browser makes it less private
than options like
[Enigmail](https://addons.mozilla.org/en-US/thunderbird/addon/enigmail/?src=search),
where the only decrypted version exists on your physical computer.

### **Chat**

There is a range of encrypted chat tools for both desktop and mobile
that can be used with your existing services (e.g., GoogleTalk) while
still encrypting and authenticating your conversations.
[Adium](https://adium.im/)

> Adium also lets you [manage contacts for multiple chat
> services](https://www.adium.im/about/) through a single interface.

for Mac and [Jitsi](https://jitsi.org/) for PC are open source and work
with most major chat services. [CryptoCat](https://crypto.cat/),
meanwhile, is both open source and Web-based, requiring only a simple
plugin installation.

On mobile, [ChatSecure](https://guardianproject.info/apps/chatsecure)
for Android works with GoogleTalk.
[SilentCircle](https://silentcircle.com/)

> Phil Zimmerman is a founder of Silent Circle.

and [Wickr](https://www.mywickr.com/en/index.php)

> Noted security researcher Dan Kaminsky and Whitfield Diffie are
> advisors to Wickr.

, have apps for both Android and iPhone that support encrypted chat as
well as encrypted text messaging and voices calls with other users of
the app.

### **Text Messaging**

A good Android solution for texts communications is
[TextSecure](https://whispersystems.org/), which supports message-level
encryption and authentication and also encrypts the texts stored on your
phone. [SilentCircle](https://silentcircle.com/) and
[Wickr](https://www.mywickr.com/en/index.php), mentioned above, also
offer encrypted text messaging.

### **Voice**

Encrypted voice and video communication over the Web depend on secure
“SIP”

> SIP, or “Session Initiation Protocol” is similar to `http`, but used
> for exchanging multimedia and voice data over the Web. Just as secure
> Web connections need to be `https`, a secure SIP service is required for
> encrypted voice services.

services, such as those supported by [ostel.co](https://ostel.co) or
[linphone.org](http://www.linphone.org/eng/linphone/register-a-linphone-account.html),
which can handle these more complex data streams. When used with these
services, [Jitsi](https://jitsi.org/) supports encrypted voice calls
from PCs, while [OSTel](https://ostel.co/about) does the same for
Android devices via the
[CsipSimple](https://code.google.com/p/csipsimple/) service.
[SilentCircle](https://silentcircle.com/) and
[Wickr](https://www.mywickr.com/en/index.php) offer encrypted voice call
support. [RedPhone](https://whispersystems.org/) also provides an
encrypted-voice option, but relies on your existing phone number, so
should not be used where unlinkability is required.ji
