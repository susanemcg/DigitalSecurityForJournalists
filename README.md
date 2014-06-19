Digital Security &amp; Source Protection for Journalists
========

**Acknowledgements**

*This paper is the product of countless conversations, encounters, recommendations and insights provided to me over the past year by members of the digital security and journalism communities.*

*Though it would be impossible to name everyone whose insight and expertise has informed this work, my deepest thanks go to Franzi Roesner, Carey Shenkman, Nabiha Syed, Seamus Tuohy, Chris Walker and Carol Waters for providing invaluable feedback and direction on early versions of this paper; your expertise and insight was invaluable. Also to Oktavia Jonsdottir, Scott Klein, Quinn Norton, Jeremy Singer-Vine and Jennifer Valentino-DeVries, who shared their ideas and work processes with me. And a very special thanks to Peter G. Neumann, who offered me the long view on digital security and directed me to essential resources and experts on the subject.*

*This project would also not have been possible without the financial and intellectual support of my colleagues at Columbia Journalism School, and the Tow Center for Digital Journalism–particularly Emily Bell and Taylor Owen. Likewise, I am very grateful to both OpenITP and TacticalTech–organizations whose generosity in hosting me in the fall of 2013 made possible so many enlightening interactions with the digital security community. Without the openness of these organizations and their associates, this work would not have been possible.*

*And finally, thanks to my talented, enthusiastic, and insightful illustrator and collaborator, Matteo Farinella, for helping make the invisible, visible.*

*First printing, June 2014*


*This paper is dedicated to all members of the digital security and journalism communities, whose shared commitment to transparency, skepticism towards power, and dedication to informing and empowering individuals everywhere has been an inspiration. I hope that this will be only the first of many collaborations between our equally scrappy, resilient, and adaptive professions.*


#Preamble


In August of 2011, the United Kingdom experienced a wave of riots that
swept across the country. The first of these took place in the Tottenham
neighborhood of London, where local resident Mark Duggan had recently
been shot and killed by police. Within hours, riots had erupted in
cities around the United Kingdom, from Manchester to Bristol, in
neighborhoods and communities with no obvious connection to the events
that took place in Tottenham. Violence, vandalism, and understandable
panic gripped the nation. In the midst of these events, the
*Guardian*–led by Simon Rogers, founder and current editor of the
Datablog–engaged in what might best be described as a real-time
investigative-reporting effort to cover not only the where, when, and
what of these riots, but also their why and how<sup>[1](footnotes/README.html#fn1)</sup>. Using social
media reports, as well as court records, extensive data analysis, and
on-the-ground reporting, the *Guardian* eventually built the story of
how these riots occurred and spread: largely through coordination
efforts facilitated by digital communications. Though the *Guardian*’s
analysis would eventually reveal–counter to the claims of Prime Minister
James Cameron–that Twitter and Facebook had played no role in spreading
the mayhem,<sup>[2](footnotes/README.html#fn2)</sup> the rioters had made extensive use of BlackBerry
Instant Messenger service to coordinate their activities. While the
*Guardian*’s analysis was sufficient to derail Cameron’s call for a “red
button” for social media, RIM–the company that then ran BlackBerry–chose
to cooperate with UK police, turning over the messages and handles
related to the events.<sup>[3](footnotes/README.html#fn3)</sup> The next month in New York, the Occupy
Wall Street movement would lead to its own set of arrests, followed by
the NYPD’s courtroom pursuit of Malcolm Harris’s Twitter
“metadata”–especially information about the location of his phone when
he posted certain tweets.<sup>[4](footnotes/README.html#fn4)</sup> Even when Twitter attempted to
*resist* cooperating with police,<sup>[5](footnotes/README.html#fn5)</sup> they were eventually forced
to turn over Harris’ data anyway.<sup>[6](footnotes/README.html#fn6)</sup> These events threw into
sharp relief the realities of privacy in the realm of digital
communications: Whether messages were privately sent or publicly shared,
users of services like BlackBerry Instant Messenger and Twitter had few
enforceable rights around the information they communicated through
these services, or even around information that the services had *about*
them. Somehow, the evolution of digital communication systems had given
rise to a strange class of information known as “metadata”: the data
*about* data that can seemingly reveal almost everything about anyone,
and yet, simultaneously, belongs to no one at all.
