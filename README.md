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

![takeover](https://user-images.githubusercontent.com/61089592/173437631-1677d46b-ee04-4453-a089-5d2e1e815561.png)

