# takeover.sh
a simple subdomain takeover in bash

#!/bin/bash

for palavra in $(cat path da wordlist);
do
host -t cname $palavra.$1 | grep "alias for"
done

usage: 

download the takeover.sh 

chmod +x takeover.sh

./takeover.sh + host (ex: google.com) 
