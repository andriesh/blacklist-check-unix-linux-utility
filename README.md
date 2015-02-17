# blacklist-check-unix-linux-utility
Blacklist check UNIX/Linux utility. I was just a bit tired of web interfaces.

###Introduction

Check blacklisting for domains and IP addresses in shell.

Works on UNIX/Linux systems with Bash.

###Installation

    curl -O https://raw.githubusercontent.com/adionditsak/blacklist-check-unix-linux-utility/master/bl
    chmod +x ./bl
    mv ./bl /usr/bin

###Usage

    $ bl domain.tld
    $ bl 8.8.8.8

###Sample output

    $ bl 8.8.8.8
    You entered an IP: 8.8.8.8
    8.8.8.8 name google-public-dns-a.google.com.
    15-02-17_Feb:02:1424185674_+0000 8.8.8.8.0spam.fusionzero.com.          [not listed]
    15-02-17_Feb:02:1424185674_+0000 8.8.8.8.0spam-killlist.fusionzero.com. [not listed]
    15-02-17_Feb:02:1424185674_+0000 8.8.8.8.rbl.abuse.ro.                  [not listed]
    15-02-17_Feb:02:1424185674_+0000 8.8.8.8.spam.dnsbl.anonmails.de.       [not listed]
    15-02-17_Feb:02:1424185674_+0000 8.8.8.8.dnsbl.anticaptcha.net.         [not listed]
    ...
