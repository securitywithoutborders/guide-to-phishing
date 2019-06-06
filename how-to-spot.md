# How to spot phishing?

Because of the fact that technological mitigations have been lagging behind, the security and privacy community have over the years devised a combination of tips that should have enabled individuals at risk to identify phishing attacks. Whether it is to look at the address bar of the browser to identify the correct domain name, or to look for the green padlock on the left of it, these recommendations are hard to follow systematically and often become obsolete (and rather dangerous) as phishing attacks evolve and as browsers evolve too.

For example, at this point, the infamous green padlock to the left of the address bar in browsers (which indicates the availability of SSL/TLS, or more simply of the ability to navigate a website over the more secure https:// instead of http://) is not a useful indicator of a legitimate website anymore. In the last years, services like [Cloudflare](https://www.cloudflare.com) and [Let's Encrypt](https://letsencrypt.org) made the adoption of SSL/TLS a lot more accessible to everyone, unfortunately including attackers launching phishing attacks (which is an inevitable downside of services that are otherwise greatly beneficial to the public.)

Similarly, checking for the right domain name in the address bar (for example, checking if "google.com" is explictly visible) might be misleading.

Both these shortcomings are well demonstrated in this example:

<blockquote class="twitter-tweet" data-lang="en"><p lang="en" dir="ltr">Quick phishing demo. Would you fall for something like this? <a href="https://t.co/phONMKHBle">pic.twitter.com/phONMKHBle</a></p>&mdash; Mustafa Al-Bassam (@musalbas) <a href="https://twitter.com/musalbas/status/1038919152826757122?ref_src=twsrc%5Etfw">September 9, 2018</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

As the video shows, while at first sight the webpage appears legitimate (there's the good old green padlock, a mark for "Secure" and the domain in the address bar appears to be "accounts.google.com"), expanding the window shows that the actual domain name was way longer ("accounts.google.com.secure.computer.shop") but hiding behind the limited view size. This trick is extremely common in real phishing attacks, and it works very well especially when targeting mobile users, because mobile browsers are necessarily limited in size and it is not trivial to inspect the expanded domain name.

Ultimately, if you know where to look and what to expect, phishing attacks can generally be identified through various visual indicators, but they can be more deceitful than you'd think! It might be useful to train your eye in recognizing anomalies, and [this quiz](https://phishingquiz.withgoogle.com) from Google might help.
