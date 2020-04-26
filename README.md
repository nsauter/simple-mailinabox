Simple Mail-in-a-Box
====================

By [@nsauter](https://github.com/nsauter) and [all contributors from the mailinabox project](https://github.com/nsauter/simple-mailinabox/graphs/contributors).

Simple Mail-in-a-Box helps individuals take back control of their email by defining a one-click, easy-to-deploy SMTP Server with a lightweight installation of only needed (and  a mail server in a box.

* * *

Our goals are to:

* Make deploying a good and simple mail server easy.
* Promote [decentralization](http://redecentralize.org/), innovation, and privacy on the web.
* **Not** make a totally unhackable, NSA-proof server.

Additionally, this project has a [Code of Conduct](CODE_OF_CONDUCT.md), which supersedes the goals above. Please review it when joining our community.

The Box
-------

Mail-in-a-Box turns a fresh Ubuntu 18.04 LTS 64-bit machine into a working mail server by installing and configuring various components.

It is a one-click email appliance. There is only one user-configurable setup option which is if you want a webmail user interface or not.. The rest "just works".

The components installed are:

* SMTP ([postfix](http://www.postfix.org/)), IMAP ([dovecot](http://dovecot.org/)), Exchange ActiveSync ([z-push](http://z-push.org/))
* Webmail ([Roundcube](http://roundcube.net/)), static website hosting ([nginx](http://nginx.org/))
* Spam filtering ([spamassassin](https://spamassassin.apache.org/)), greylisting ([postgrey](http://postgrey.schweikert.ch/))
* DNS ([nsd4](https://www.nlnetlabs.nl/projects/nsd/)) with [SPF](https://en.wikipedia.org/wiki/Sender_Policy_Framework), DKIM ([OpenDKIM](http://www.opendkim.org/)), [DMARC](https://en.wikipedia.org/wiki/DMARC), [DNSSEC](https://en.wikipedia.org/wiki/DNSSEC), [DANE TLSA](https://en.wikipedia.org/wiki/DNS-based_Authentication_of_Named_Entities), and [SSHFP](https://tools.ietf.org/html/rfc4255) records automatically set
* Backups ([duplicity](http://duplicity.nongnu.org/)), firewall ([ufw](https://launchpad.net/ufw)), intrusion protection ([fail2ban](http://www.fail2ban.org/wiki/index.php/Main_Page)), system monitoring ([munin](http://munin-monitoring.org/))

It also includes:

* A control panel and API for adding/removing mail users, aliases, custom DNS records, etc. and detailed system monitoring.

For more information on how Mail-in-a-Box handles your privacy, see the [security details page](security.md).

Installation
------------

See the [setup guide](https://mailinabox.email/guide.html) for detailed, user-friendly instructions.

For experts, start with a completely fresh (really, I mean it) Ubuntu 18.04 LTS 64-bit machine. On the machine...

Clone this repository:

	$ git clone https://github.com/nsauter/simple-mailinabox
	$ cd simple-mailinabox

Begin the installation.

	$ sudo setup/start.sh

For help, DO NOT contact Josh directly --- I don't do tech support by email or tweet (no exceptions).

Post your question on the [discussion forum](https://discourse.mailinabox.email/) instead, where maintainers and Mail-in-a-Box users may be able to help you.

Contributing and Development
----------------------------

Mail-in-a-Box is an open source project. Your contributions and pull requests are welcome. See [CONTRIBUTING](CONTRIBUTING.md) to get started. 


The Acknowledgements
--------------------

This fork project was obviously inspired by ["Mail-in-a-Box"](https://github.com/mail-in-a-box/mailinabox) and does benefit from already done development by all contributors.

Mail-in-a-Box is similar to [iRedMail](http://www.iredmail.org/) and [Modoboa](https://github.com/tonioo/modoboa).

