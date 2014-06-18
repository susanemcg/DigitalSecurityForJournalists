Where Unlinkability Is A Necessity
----------------------------------

Creating unlinkable digital communications first requires understanding
what our digital communications networks see, as was discussed in detail
in the previous section. The next step is to evaluate exactly what level
of unlinkability a given situation requires. Is it important that the
source not be linked to a *particular* journalist, or is it dangerous
for the source to be seen communicating with any journalist at all? Is
having this person remain truly anonymous–meaning his or her physical
and/or legal identity is unknown even to the reporter–an option, either
technically or journalistically speaking? What are the physical,
technical, legal, financial, and expertise constraints of both parties?

The next step is to consider the data streams that can be used to
connect our digital activity to our real identities. Our Web browsers
and even operating systems are littered with flecks of digital DNA;
accounts that require logins–like email, social networks and online
marketplaces–tether these digital identities to our physical identities
through recognizable handles and financial details. Our network
connection points are often linked to our physical selves as students,
cable account holders, and employees.

Creating unlinkable communications, then, means creating an environment
where these traces are either eliminated or obfuscated, from our
operating systems up through our online accounts. Fortunately, some
good, open-source tools exist that can be composed along with some solid
strategies to make this feasible.

### **Unlinkable Web Browsing: Tails + Tor**

The simplest way to make sure that your computer is “sanitized” of any
identifiable digital traces is simply to do as a doctor would: Dispose
of your operating system after every use. Though impractical for
everyday tasks where you need to be able to regularly store, modify, and
share files, this “discard after use” approach is exactly the system
design of [Tails](https://tails.boum.org/)–a Linux-based operating
system that lives on a USB drive and can be run directly from that drive
on any computer available. When the computer is restarted, Tails starts
up only in the host machine’s random access memory (RAM) and deletes
itself on shutdown. Because Tails is recreated from scratch every time
it is started, it can’t leak identifying bits of digital debris when you
connect to the Internet.

> Ideally, you should not store files on your Tails USB drive, with the
> possible exception of your GPG key. The Tails documentation provides a
> good overview of [what Tails + Tor can and cannot
> protect.](https://tails.boum.org/doc/about/warning/)

Unfortunately, the mechanics of the Internet *require* that a fair
amount of identifying information be attached to our digital
communications, simply in order to function. In some ways the most
stubborn of these identifiers is our IP address, which maps to the
physical location of our Internet connection. While it may be easy to
imagine creating “throwaway” email accounts to use with a source,
influencing IP addresses seems generally beyond our control.

Enter Tor, or “the onion router.” Best known for its [well-used (and
very usable)
browser](https://www.torproject.org/projects/torbrowser.html.en), Tor is
a combination of special Internet nodes (“relays”) and software designed
to effectively mask the IP address of your Internet traffic. It
accomplishes this by wrapping each packet of your Web traffic–including
its “to” and “from” metadata–in three successive layers of encryption;
it then hands off these encryption-wrapped packets to its exclusive
network.

Your packets then move across three nodes in the Tor network, each of
which has the ability to “peel off” exactly one layer of encryption; by
the time your data reaches the final “exit” node–whose IP address it
will take on–it has been “unwrapped” to its original state and can make
its way on the open Web just as it would with your regular Internet
connection. The result is that, to outside observers, your Web traffic
seems to be coming from an IP address (and therefore physical location)
other than your own.

Tor is designed not only to protect your data from being traced by
outside parties, but also from monitoring by the Tor network itself. Not
only is your content encrypted, but each node only knows the location of
the immediately previous node in the Tor communication chain. In
addition to this, Tor cycles the set of relays your traffic uses
approximately every 10 minutes, so that analyzing your pattern of
Internet traffic for other identifying information is more difficult to
do.

> For more detail, see the [Tor
> overview](https://www.torproject.org/about/overview.html.en)

While Tor is often described as an “anonymity” network, it offers a very
particular *type* of anonymity: locational anonymity for your Web
traffic, nothing more. While it does this very well, using Tor does not
obfuscate *what* you are doing on the Web, only *where* you are doing it
from. If you log-in to Facebook–or Google or Yahoo or Twitter or what
have you–those services will still have records of your activity as they
always would; it’s just that the IP address they see won’t match where
you really are. Likewise, using Tor Browser doesn’t automatically
protect you from cookie-based tracking; you need to make sure that
cookies are turned off.

Two final points about Tor: The addresses of Tor relays are not secret.
In fact, having them known is part of what makes it possible to perform
checkups that assure the network isn’t compromised. This does mean,
however, that anyone observing your Web traffic will know that you’re
using Tor, either because they see your traffic going *in* to a known
Tor relay or coming *out* of a known exit node. There is nothing illegal
about using Tor. In fact, the more that people use Tor for regular Web
browsing, the better its obfuscation properties work. That said,
depending on where you are, connecting to the Tor network may make your
Web traffic stand out. If you think the network operator (or the state)
may be watching your traffic, using Tor may not be a good idea.
Remember, all security is situationally dependent; there is no
substitute for knowing your context.

Second, Tor is a *low-latecy* (i.e. minimal-delay) network, meaning it
passes your packets back and forth as quickly as possible.

> “Mix-nets” are [*high-latency* networks that send out messages in
> batches](http://ritter.vg/blog-mix_and_onion_networks.html), making it
> difficult to identify their destination.

While this is part of what makes it a viable alternative to more
mainstream browsers like Firefox and Chrome, it does mean that someone
watching both your IP address and the correct exit node stands a good
chance of being able to connect it back to you. Although your connection
going into the Tor network is encrypted, if this encryption were
penetrated, experiments have shown that over time someone watching both
the entering and exiting streams of traffic could statistically connect
the two. However, because this type of traffic analysis is at least
[legally
restricted](https://www.torproject.org/docs/faq.html.en#AttacksOnOnionRouting)
in many places this risk is most salient when you are on a private
and/or state-controlled (e.g., company, university and some national)
network.<sup>[46](footnotes/README.html#fn46)</sup>

### **Unlinkable Email: Keep Your Pseudonyms Isolated**

Any time you communicate with a source via email or chat, you are both
necessarily communicating either with a *pseudonym* which may or may not
be *linkable* to your “real,” or physical, identity. In some cases, it
may be important that both you and your source use *unlinkable*
pseudonyms; this will help protect your sources in the case that being
known to communicate with a journalist (or with you specifically) may
put them at risk. If this is not the case, however, it may be sufficient
for your source to use an unlinkable email address or handle for a
particular exchange.

In order for unlinkable email to work, the address or handle itself must
be created in an unlinkable context (e.g. an email account that you
create and access only via [Tor
Browser](https://www.torproject.org/projects/torbrowser.html.en)), and
you must both be vigilant not to include identifying information in the
account details, or share any information that might connect the account
to real individuals or locations. This means not discussing anything
personally identifying: physical location, local stores, workplace name,
or friend or family connections.

> [Lantanya Sweeney](http://latanyasweeney.org/index.html)’s
> foundational [work on
> identifiability](http://latanyasweeney.org/work/identifiability.html)
> demonstrated that 87% of Americans could be identified by [a
> combination of zip code, gender and date of
> birth.](http://dataprivacylab.org/dataprivacy/projects/kanonymity/kanonymity.pdf)

Remember that unless the contents of your chat or email are encrypted,
this information could be accessed by third parties (e.g., your email
provider or law enforcement) and used to connect these communications to
your real identities.

Likewise, your unlinkable identities themselves cannot be exchanged via
any linkable communication channel (e.g., unencrypted, linkable email or
chat accounts). You *must* agree upon and exchange these identities by
some means outside of the communication channel you wish to use.
In-person exchanges are best, human networks (trusted mutual
acquaintances), voice conversations (for an existing source), and
physical mail exchanges are also reasonable options.

> Postal mail services are a viable option for many reasons: the
> physical & legal protections are better, as is the obfuscation - a
> great deal of postal mail still moves through the system each day.

You will have to judge which of these is the best approach for a given
situation on a case-by-case basis.

### **Unlinkable Chat**

Unlinkability in synchronous (real-time) communications like chat is
easier than with asynchronous communications like email; it actually has
the potential for [*perfect forward
secrecy*](https://www.eff.org/deeplinks/2013/08/pushing-perfect-forward-secrecy-important-Web-privacy-protection).
A chat service used with an unlinkable handle that is accessed on a
[Tails](https://tails.boum.org/) computer and/or through [Tor
Browser](https://www.torproject.org/projects/torbrowser.html.en) is
particularly robust. Any of the encrypted-chat applications mentioned
above can be used in this environment, though ones like
[CryptoCat](https://crypto.cat/), which don’t require saving any
information to [Tails](https://tails.boum.org/), are preferable in these
instances.

### **Unlinkable Text**

Many encrypted text programs actually use your mobile phone’s data
connection to send messages, but most of them read your contact
information and will (necessarily) show the phone number of the sender
and recipient along with the message. While
[TextSecure](https://whispersystems.org/) supports perfect forward
secrecy, chat is often a better option for unlinkable exchanges.

### **Unlinkable Voice**

As with text, encrypted voice calls are actually carried over your data
connection. Apps like [OSTel](need%20link) use a number different than
your regular phone number, as do apps like
[SilentCircle](https://silentcircle.com/) and
[Wickr](https://www.mywickr.com/en/index.php). Though some reporters may
use so-called “burner phones,” obtaining and using any kind of mobile
device in such a way that it cannot be connected to your identity is
nearly impossible. Stick with computer-based voice calls or go back to
good old-fashioned postal mail.