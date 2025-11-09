1. grep -q routerich /etc/opkg/customfeeds.conf || echo src/gz routerich https://github.com/routerich/packages.routerich/raw/24.10.3/routerich >> /etc/opkg/customfeeds.conf
2. wget https://github.com/routerich/packages.routerich/raw/main/routerich.pub -O /tmp/routerich.pub && opkg-key add /tmp/routerich.pub
3. opkg update
