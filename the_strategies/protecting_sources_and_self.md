Protecting Your Sources, Protecting Yourself
--------------------------------------------

At the heart of most U.S. shield protections for journalists is a simple
premise: If journalists cannot protect their sources, it substantially
harms their ability to obtain the information they need to hold
government accountable–perhaps the fundamental objective of a free and
independent press. Given the current legal and technical realities,
however, journalists who communicate with their sources digitally may be
rendering these protections essentially moot. In practice the defaults
on most email, chat, text, and telephone systems effectively identify
our sources with every exchange, so protecting them means successfully
scattering these digital traces so they cannot be used to connect the
dots.

Of course, we work with many sources whose connection to us can be, and
is, acceptably known, through long association or publication. Yet
communication with these sources needs protecting too. As every
journalist knows, sources sometimes don’t appreciate the implications of
the information they share; ensuring confidentiality of their
communications with us is an important part of source protection even if
their identity is public.

Because of this, you’ll find the content below broken broadly into two
sections: strategies for protected but *linkable* communications,
followed by strategies for *unlinkable* communications. First, however,
we’ll address the three main methods of digital information protection:
encryption, obfuscation, and deletion.

### Encryption

Put simply, encryption is the process of scrambling or encoding messages
in such a way that only someone with the correct “key” can unlock or
unscramble the original.

In digital communications, there are two primary types of encryption:
*symmetric* and *asymmetric*. In symmetric encryption, a single, secret
key is used to both encrypt and decrypt a message. This approach is
strong and fast, but requires that sender and recipient somehow agree
on–and *securely* share–a single secret key. Symmetric encryption has
been used for thousands of years and, at its heart, is very similar to
the kinds of alphabetic substitutions that you might find on a decoder
ring.

*Asymmetric* encryption, on the other hand, works by generating a
mathematically related “public-private” key *pair*. Though each key can
decode a message encrypted by the other, the two keys are asymmetric in
the sense that the public key can be generated from the private key, but
not the reverse. How is this possible? Asymmetric encryption takes
advantage of the fact that it is generally much easier to mix things
together than it is derive the original components from the finished
product. For example, it is easy to create some color of green paint by
mixing together yellow and blue. But the only way to tell what
proportion of yellow and blue paints went into making a particular shade
of green is through a long and arduous process of trial and error.

In mathematics, multiplication is fast, but factoring is
time-consuming–even for a computer. The only way to find the factors of
a number is to work your way up the number line, testing every
possibility as you go. Public-private key pairs are based on this
principle: The private key consists of a unique set of factors that when
multiplied together yield the public key. Use enough factors–preferably
prime numbers–in your private key, and it would take today’s computers
decades or more to derive the private key from the public one.

These special properties of public-private key pairs let us do things
with them that we cannot do with symmetric keys. For example, we can (as
the name suggests) make the public key *public*, and claim it openly on
the Web. Anyone who wants to send us an encrypted message can encode it
with our public key, knowing that *only* the owner of the private key
can decode it. Likewise, by sharing a message encoded with our *private*
key, we let others verify that the public key we have indicated truly
belongs to us. Of course, knowing that a person controls a particular
key pair doesn’t actually tell you *who* they are. That step–confirming
the “real” identity of the person who controls a particular key–is known
as *authentication*.

For individuals, authentication can be done by *securely* sharing the
*hash* (sometimes also called called a “fingerprint”) of your public
key.

> A typical PGP hash is 32 characters long.

Most simply, this can be done in person, via business card or QR code.
Voice authentication is also a good option, since we tend to recognize
individuals’ voices. Even postal mail can be an option, if you’re
confident about where to physically reach the person with whom you’re
trying to communicate. For websites, third parties vouch for the
legitimacy of a public key by “signing” (or authenticating) it with
their own. This is the equivalent of believing your friend when he or
she gives you someone’s email address.

In practice, virtually all digital encryption systems are *hybrid*
systems: They use both symmetric and asymmetric encryption. Typically,
this means encrypting the actual message with a unique symmetric key,
and then encrypting the symmetric key itself with the appropriate public
key and transmitting it with the message. This is the process that
underlies both secure () Internet connections and encrypted email.

> A website’s “security certificate” is just another name for its public
> key.


There are cases, however, where no already-known “public key” is
available to encrypt that symmetric key; when connecting to a wireless
router, for example, or using many secure chat programs. For these, keys
must be generated and exchanged on the fly, using a process called
Diffie-Hellman key exchange.

> For a helpful demonstration of this type of exchange, see [Chris
> Bishop’s segment for the *Royal Institution Christmas
> Lectures.*](http://www.youtube.com/watch?v=U62S8SchxX4)

Despite the fact the fact that the first messages are exchanged “in the
clear,” this process makes it possible for both devices to derive the
same shared secret key.

There is a vulnerability here, of course. How does one know that the
*first* message really came from the person you think it did? If you had
a public key to compare it to, it would be easy to check. Without this,
however, it is possible that a third party could intercept your
communications and impersonate each side to the other–all the while
decrypting and reading all of the messages you exchange. This is known
as the “Man in the Middle” (MITM) attack.

Fortunately, the MITM attack is simple to thwart: Simply telephone the
person with whom you are chatting to verify that your secret keys match
(many programs will display them on screen), or exchange it via
encrypted email (provided you’ve already or *authenticated* that the
public key you have really belongs to them). After that, you can chat
with confidence.

### Obfuscation

*Obfuscation* is exactly what it sounds like: digitally “hiding”
information, whether it’s data stored on your computer or your IP
address on the Internet. Some forms of obfuscation also provide
“plausible deniability”; in other words, the reasonable appearance that
nothing is being hidden.

In general, obfuscation is difficult to do on one’s own; its
effectiveness depends primarily on your data’s ability to “blend in.”
For example, using “hidden volumes” to make an archive of sensitive
documents *look* like a movie file works best if you have a reasonable
number of movie files on your computer. That way, the chances of an
attacker locating the one that is not actually a movie is much lower.
Similarly, using a VPN or Tor to mask the geographic origin of your
Internet traffic (addressed shortly) works best if there are many other
users on the same system. In this sense, obfuscation can be best
understood as a kind of herd protection, much like digital security in
general. The bigger the crowd your data or operations can blend into,
the more difficult it makes you and your sources to target.

One of the common challenges to the suggestion that more people use
encryption is that there are environments where it makes one stand out,
and thus a target for greater scrutiny. There are many cases where this
is true. Obfuscation is exactly the principle of “security by
obscurity,” which may actually mean *forgoing* encryption in certain
contexts.

### Deletion

Ultimately, no kind of search can expose information you don’t have,
both for individuals and service providers. Regularly and securely
deleting unnecessary emails and files, especially from hosted services,
is a simple and effective protection against having your data rifled
through either by the authorities or by hackers. Think of this as
cleaning out your file cabinet on a regular basis: Do it once every
three months to help keep your exposure in check.

> Recall that the contents of emails over 180 days old may be subject to
> subpoena, so doing this every six months is a minimum.

And remember that simply “trashing” your information isn’t enough.
Online you’ll need to “delete forever,” and on your computer you’ll want
to use a tool like [CCleaner](http://ccleaner.en.softonic.com/) to truly overwrite
“deleted” files so the data can’t be retrieved.