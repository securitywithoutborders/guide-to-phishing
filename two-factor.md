# Two-factor authentication

An attempted mitigation to phishing has been developed over the years and many (although likely not most) have by now enabled what is commonly referred to as **two-factor authentication**, **two-factor verification**, **two-step verification**, etc. The basic idea is quite simple: because passwords can be stolen or guessed, you will be required to perform a secondary verification that should prove your ownership of the account for which a login is being attempted.

Different websites offer implement different flavors of two-factor authentication, but most commonly they come in the following forms:

1. **SMS verification**: After having successfully entered your credentials, the service (such as Google, Yahoo, Facebok, or Twitter) will send an SMS message to the phone number you provided upon registration, containing a token (generally numerical or alphanumerical) which you will be required as well to enter in the login page.
2. **Authenticator apps**: When you enable two-factor authentication, some services will ask you to install a mobile app on your phone which you will be required to open when attempting a login to fetch a short-lived numerical or alphanumerical token to enter in the login page, very similarly to the previous option.
3. **Push notification**: When you enable two-factor authentication, some services will ask you to install a mobile app which will automatically send you a notification when a login to your account is attempted, and if you wish to authorize it you'd just need to tap a button.

Without any doubt, these forms of two-factor verification are helpful mitigations that could thwart casual attackers from being able to illegitimately access your accounts. These procedures can be particularly effective against non-targeted phishing attacks (more simply, the kind of attack that would be sent to people en masse through spam emails) and against password reuse (which could be a very real risk considering the [many data breaches](https://www.haveibeenpwned.com) we keep learning about.)

However, **these forms of two-factor authentication are not a solution to *all* phishing**. If an attacker is sufficiently resourceful (and many are) they can automate their phishing platform to effectively bypass two-factor verification. Quite simply, if you have fallen for such an attack and have already provided your username and password, the attackers can simply solicit a valid token from you just in the same way. They would then automatically use the token before it expires, and successfully log into your account.

For example, following is a screenshot of a phishing site soliciting a verification code that was sent via SMS:

![](img/gmail-2fa.png)

This is not hypotethical. We have seen several cases of large-scale targeted phishing campaigns that have employed this technique. For example in the following reports:

- [When Best Practice Isn't Good Enough: Large Campaigns of Phishing Attacks in Middle East and North Africa Target Privacy-Conscious Users](https://www.amnesty.org/en/latest/research/2018/12/when-best-practice-is-not-good-enough/) by Amnesty International
- [The Return of The Charming Kitten](https://blog.certfa.com/posts/the-return-of-the-charming-kitten/) by CERTFA.

**Please note**: this is not to say that those forms of two-factor authentication are useless. Not at all. [If a service you are using provides any of those options to you](https://twofactorauth.org/), make sure to enable it as it is nevertheless a useful additional layer of security. However, if you are an individual at risk, who might especially be targeted by persistent attackers, you might want to explore additional options (such as those explained later) and generally exercise a lot more caution.
