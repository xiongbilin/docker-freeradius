## Requirement
+ Docker 0.11

## Usage
1. configure

    ```bash
    # assets/install.sample.sh (Rename to install.sh after you're done)
    radpass='Your Radpass'
    mysql_server='Your Mysql Server ip or Address'
    mysql_login='Your Mysql Username'
    mysql_passwd='Your Mysql Password'
    ```

2. run ```build.sh``` and ```run-server.sh``` 

3. if freeradius is linked to MySQL on localhost, maybe you'd like to add an iptables rule like:
    ```ufw allow proto tcp from 172.17.0.0/16 to any port 3306```

## Note
+ all remote freeradius clients (ipv4/ipv6) are allowed
+ ```default_eap_type = mschapv2 (default: md5)``` in ```/etc/freeradius/eap.conf```

## Reference
+ TBD


