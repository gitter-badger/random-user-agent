# Random User-Agent

![Release version][badge_release_version]
![Chrome WebStore version][badge_websore_version]
![Chrome WebStore rating][badge_websore_rating]
![Commits since latest release][badge_commits_since_release]
![License][badge_license] 

Automatically replaces the User-Agent after a specified time interval

![Screenshot][screenshot]

### Warning

Depending on your threat model, faking your user agent might make you _more_ fingerprintable, not less. There are ways other than `User-Agent` sniffing to determine what browser you're using, so malicious sites could learn what browser you're _really_ using through other means and then combine that with your randomly changing `User-Agent` to pretty effectively track you. For background, see [this GitHub issue](https://github.com/tarampampam/random-user-agent/issues/47). You've been warned.

### Get the Plugin! [Google Webstore] & [Firefox Add-ons]

User-Agent - a string that is sent along to any website you visit. This is a sort of "fingerprint" your browser leaves behind which contains:
- The name and version of your browser;
- The name of the operating system (Mac, Windows, Linux, etc.) and its version;
- Information about some of the plugins installed on the browser;
- Other information that identifies and exposes you.

This extension has been created to stop data leakage. It automatically replaces User-Agent strings after a specified period of time with a randomly selected one. User-Agent strings can also be set manually. The extension is incredibly lightweight, using very few resources. User-Agent randomization can be customized by the user (what browsers and OS are spoofed, etc.). Exceptions list available with option of wildcards. Protects against Javascript exploits to hide your identity and protect your anonymity.

> Thanks to SmudgedMuffin for English localization, and [@nazarpc](https://github.com/nazar-pc) for Ukrainian localization

### Building from sources

For a building extension from sources _(and pack as a `zip` file)_ use next commands:

```bash
$ cd /path/to/the/sources
$ gulp
```

> You can install `gulp` globally with next command: `$ sudo npm install -g gulp`

[badge_release_version]:https://img.shields.io/github/release/tarampampam/random-user-agent.svg?style=for-the-badge&maxAge=5
[badge_websore_version]:https://img.shields.io/chrome-web-store/v/einpaelgookohagofgnnkcfjbkkgepnp.svg?style=for-the-badge&maxAge=5
[badge_websore_rating]:https://img.shields.io/chrome-web-store/rating/nimelepbpejjlbmoobocpfnjhihnpked.svg?style=for-the-badge&maxAge=5
[badge_commits_since_release]:https://img.shields.io/github/commits-since/tarampampam/random-user-agent/latest.svg?style=for-the-badge&maxAge=5
[badge_license]:https://img.shields.io/github/license/tarampampam/random-user-agent.svg?style=for-the-badge&maxAge=30
[link_create_issue]:https://github.com/tarampampam/random-user-agent/issues/new
[screenshot]:https://raw.githubusercontent.com/tarampampam/random-user-agent/master/webstore_content/slides/slide-1.jpg
[Google Webstore]:https://chrome.google.com/webstore/detail/random-hide-user-agent/einpaelgookohagofgnnkcfjbkkgepnp
[randexp.js]:http://github.com/fent/randexp.js
[Firefox Add-ons]:https://addons.mozilla.org/firefox/addon/random_user_agent/
