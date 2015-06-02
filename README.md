# mailgraph SPF DMARC DKIM patch

This patch was found at https://www.kernel-error.de/postfix/mailgraph-aufgebohrt

I only added it here to have a copy :)

Testet at mailgraph Version 1.14

Patch:

    patch -p0 /usr/sbin/mailgraph < mailgraph.patch
    patch -p0 /path/to/mailgraph.cgi < mailgraph.cgi.patch

Then remove the old .rrd files from (on Debian):

    rm  /var/lib/mailgraph/*.rrd

restart mailgraph:

    service mailgraph restart
