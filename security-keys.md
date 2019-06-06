# Security keys

Currently, security keys are the most secure form of two-factor authentication. Security keys are hardware tokens that implement what is known as the [U2F protocol](https://en.wikipedia.org/wiki/Universal_2nd_Factor) and they generally come in the shape of USB keys, although some support other channels such as NFC (mostly to function with mobile devices). When an online account is protected using a security key, the user is required not only to enter their password but to physically insert the security key in the device. This process is nicely visualized in the following animation taken from the [Solo](https://www.kickstarter.com/projects/conorpatrick/solo-the-first-open-source-fido2-security-key-usb) Kickstarter campaign:

![](img/solo.gif)

While in the case, for example, of SMS verification an attacker could steal the verification code sent to the user, in this case the attacker can only physically steal the security key (as well as obtain the password) in order to log into the target's account. Obviously, this is significantly harder.

More considerations on two-factor authentication and security keys are available in [this post](https://www.amnesty.org/en/latest/research/2018/12/when-best-practice-is-not-good-enough/) from Amnesty International:

> This technology is supported for example by Google's Advanced Protection program, by Facebook and as of recently by Twitter as well. This process might appear painful at first, but it significantly raises the difficulty for any attacker to be successful, and it isn't quite as burdensome as one might think. Normally, you will be required to use a security key only when you are authenticating for the first time from a new device.

> That said, security keys have downsides as well. Firstly, they are still at a very early stage of adoption: only few services support them and most email clients (such as Thunderbird) are still in the process of developing an integration. Secondly, you can of course lose your security key and be locked out of your accounts. However, you could just in the same way lose the phone you use for other forms of two-factor authentication, and in both cases, you should carefully configure an option for recovery (through printed codes or a secondary key) as instructed by the particular service.

There are numerous companies producing these security keys. When you shop for one, make sure that your selected option explicitly supports U2F. Some of the options we recommend are:

- [YubiKey](https://www.yubico.com/product/security-key-by-yubico/)
- [NitroKey](https://www.nitrokey.com/)
- [SoloKeys](https://shop.solokeys.com/) (open hardware and open source)
