Beyond the Exchange: Data Security in the Cloud
-----------------------------------------------

### Understanding Email

Thinking of messages sent over `http` as postcards and those sent via `https` as
letters in envelopes is actually a fairly good analogy for how your
information is and isn’t exposed when you’re actively sending messages
to and from a website. But what about after that exchange has ended? At
least some of the information we exchange with websites–be they
financial websites, social networking services, or email providers–ends
up being stored by them for various purposes. Obviously, any website
that requires a username and password will need to store those in order
to protect your account. Social networking services host copies of our
posts and photos; financial institutions retain records of our accounts
and transactions. Email providers that offer Web-based email access
maintain copies of our emails.

While all of this is to be expected, the way this information is
*treated*, both legally and technically, may not always meet our
expectations. For example, it is generally regarded as good practice to
store passwords only in encrypted form in case of a security breach,
though leak incidents demonstrate that not all service providers adhere
to this security rule of thumb.<sup>[38](footnotes/README.html#fn38)</sup> To protect your information
from outside attackers, financial institutions and email providers also
typically encrypt the copies they maintain of your account information
and emails. At the same time, these companies have the ability to
*decrypt* your information as well; if they didn’t, opening an email on
the Web would only reveal encrypted gibberish, rather than the readable
text of the note that your best friend sent you this morning

> Google’s [recent “end-to-end”
> offering.](http://googleonlinesecurity.blogspot.com/2014/06/making-end-to-end-encryption-easier-to.html)
> may address some of these issues, but further analysis is needed to
> assess exactly how the library works.

Obviously, this is part of what makes Web-based email services so
convenient–we can read and refer to our email from anywhere.

The flip side of this convenience, however, is that your email provider
has as much capacity as you do to access the readable text of the note
your friend sent to you. If their servers are successfully hacked, the
attacker will be able read all of your emails as well. Perhaps more
likely–though arguably equally problematic–there are many cases where
your email provider may be compelled to use its access to provide the
text of your email messages to requesting authorities.<sup>[39](footnotes/README.html#fn39)</sup> This
capacity can also be leveraged by law enforcement to compel an email
provider to decrypt and share emails and other information that is more
than 180 days old, because these are considered “abandoned” and so can
be legally obtained through a subpoena–contents and all ([18 U.S.C.
2703(a)](http://www.law.cornell.edu/uscode/text/18/2703)).

### Understanding Endpoints

Even without recurring headlines of cybercrime, attacks on Web servers,
and security breaches, it probably seems commonsensical that businesses
would use encryption to protect the data they store. After all, a bank’s
website is as obvious a target for a criminal attack as a
brick-and-mortar branch would be; perhaps even more so given that it can
be accessed from anywhere and is likely a conduit to a much greater
volume of assets. Not encrypting sensitive organization and customer
information would be an obvious security hole.

But the data on your computer doesn’t need to be a gateway to millions
of dollars in order to have value to an attacker. Journalists and those
close to them may be the targeted for the information that their devices
contain about both sources and stories: contact lists, interview notes,
source documents, etc. Even for non-journalists, gaining access to your
device can be valuable to the authorities or a criminal seeking
information, since many of us store passwords or sensitive financial and
medical information on our computers and phones.

In security-speak, an “endpoint” is any device that stores information.
In this sense, Web-service providers’ servers are endpoints; so is your
laptop or mobile phone. Protecting them generally requires following
some simple rules: Don’t leave them in a situation where others can gain
physical access to them; and to be on the safe side, encrypt them. We
are apart from our devices more than we may readily imagine, whether to
use the bathroom at a coffee shop or pass through a security checkpoint
at an airport. Probably the most common and high-profile example of the
latter situation was exemplified when Glenn Greenwald’s partner, David
Miranda, flew through London Heathrow Airport in August of 2013; his
computers and hard drives were taken from him for several
hours.<sup>[40](footnotes/README.html#fn40)</sup> Any unencrypted information they contained would
have been readily accessible to authorities. Just because you have a
password on your computer or phone doesn’t mean its contents are
encrypted; this is something you need to set up explicitly.

### Don’t Get “Pwned”

That said, encryption will not protect your data against malicious
software that you have voluntarily (if unknowingly) loaded onto your
device yourself.

> The term “pwn” (pronounced p'ōn) derives [either from World of Warcraft or
> chess.](http://www.wowwiki.com/Own)

This most commonly happens through USB drives and downloads, both of
which may contain hidden programs designed to access, manipulate, and/or
communicate your private information whenever you next connect to the
Internet. Trusting the source of the device or document isn’t enough to
protect you. Brand-new USB drives have been known to have malware
embedded by their manufacturers, and documents that can run
programs–such as PDFS–may contain malware of which even the sender is
unaware. This doesn’t mean that working with these resources is
impossible, but it does require taking some simple precautions. One such
approach is opening potentially problematic filetypes in a service like
Google Docs first; these services are built to scan for and eliminate
malware. Another approach is to set up an “air gapped” computer, which
is simply an old machine that you never let connect to a network. This
way, any malicious software is starved of the connection it needs to
leak information. Of course, the first option only makes sense if the
information is not sensitive; anything you save to Google Docs (or a
similar Web-based service provider) falls under the same legal and
technical rules of access as those described for email above.