# [mutt-config](https://github.com/ishbguy/mutt-config)

[![License][licsvg]][lic]

[licsvg]: https://img.shields.io/badge/license-MIT-green.svg
[lic]: https://github.com/ishbguy/mutt-config/blob/master/LICENSE

![mutt-config-screenshot](https://github.com/ishbguy/mutt-config/blob/master/screenshots/mutt-config-screenshot.png)

## Table of Contents

+ [:art: Features](#art-features)
+ [:straight_ruler: Prerequisite](#straight_ruler-prerequisite)
+ [:rocket: Installation](#rocket-installation)
+ [:memo: Configuration](#memo-configuration)
+ [:hibiscus: Contributing](#hibiscus-contributing)
+ [:boy: Authors](#boy-authors)
+ [:scroll: License](#scroll-license)

## :art: Features

+ Vim like navigation
+ Tree view mailboxes
+ Pragmatic style status, index, pager formats string
+ Kindly colorscheme

## :straight_ruler: Prerequisite

> + `offlineimap`: Fetch and download e-mails from remote mail server.
> + `msmtp`: Send e-mails.
> + `procmail`: Filter e-mails.
> + `notmuch` & `notmuch-mutt`: Search local e-mails.
> + `abook`: Maintain e-mail addresses and aliases.
> + `urlview`: Browser url in e-mails.
> + `aview`: Covert pic to asicii art.
> + `lynx` & `w3m`: View html style mails.

## :rocket: Installation

```bash
$ git clone https://github.com/ishbguy/mutt-config ~/.mutt
```

## :memo: Configuration

+ Add email config and generate `offlineimap`, `msmtp` and `mutt-accounts` configurations:

```bash
$ # config file name  must end with .ac
$ cat <<EOF >~/example.ac
realname="your realname"
account=yourname@example.com
recv_host=imap.example.com
send_host=smtp.example.com
password=your-password
EOF
$ ~/.mutt/bin/mutt-genconfig.sh ~/example.ac
$ # download mails
$ offlineimap
```
After the above operations, you can type `mutt` to enjoy reading your mails.

## :hibiscus: Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## :boy: Authors

+ [ishbguy](https://github.com/ishbguy)

## :scroll: License

Released under the terms of [MIT License](https://opensource.org/licenses/MIT).
