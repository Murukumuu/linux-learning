Syntax: find [path] [tests/conditions] [actions]
E.g find / -type f -size 33c -user bandit7 -group bandit6 2>/dev/null
File size: bytes - c, Kib - k, MiB - M, GiB - G
Notes
locate files based on properties like name, size, permissions, or owner.
/ is to search root
2>/dev/null is to hide denied errors

Syntax: grep [options] "word_or_pattern" [file]
E.g grep "millionth" data.txt
Notes
looks for words inside file
-i to ignore capitalization 
-n to display word line numbering

Syntax: sort [file] | uniq -u
E.g sort data.txt | uniq -u
Notes
sorts file alphabetically 
-u to highlight unique words (per)
uniq -u to filter and highlight words

Syntax: string [file]
Notes
scans file and extracts only human readable parts

Syntax: base64 [options] [file]
Notes
use --help

Syntax ROT13: tr 'A-Za-z' 'N-ZA-Mn-za-m' <<< "Pack My Box With Five Dozen Liquor Jugs", echo "The Quick Brown Fox Jumps Over The Lazy Dog" | tr '\!-~' 'P-~\!-O'

IMPORTANT
Restore DNS = ping google.com (verify dns working), sudo systemctl restart systemd-resolved, sudo systemctl status systemd-resolved
Restart dhclient = ip link, sudo ip link set ens33 up (change status of ip link), sudo dhclient -v ens33 (assign ip and dns info)

