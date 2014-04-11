apli_cnc
========

Command and control for web apps based on apli_template

Installation and Setup
----

``` sh

git clone
cd apli_cnc
virtualenv --no-site-packages .
. bin/activate
pip install -r requirements.txt
    
echo 127.0.0.1 >> ansible_hosts
alias APLI="ansible -i `pwd`/ansible_hosts --private-key=~/.ssh/id_rsa all"
APLI -m setup
```

