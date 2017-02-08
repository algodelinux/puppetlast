puppetlast
==========

Overview
--------

This program shows the last connect time of puppet nodes.  
It currently displays them in green if they've connected in seconds or minutes.  
It currently displays them in red if they've connected in hours or days.  
The program need gawk for working. So it will install gawk if it isn't installed.

Installing
----------

You can install it simply running these commands on your puppetmaster::

   $ wget --no-check-certificate -O /usr/local/sbin/puppetlast https://github.com/algodelinux/puppetlast/raw/master/puppetlast  
   $ chmod 755 /usr/local/sbin/puppetlast 

Using
-----

Syntax: puppetlast [-m|--min time] [-M|--max time]

Options:  
 -m|--min: let specify min display time
 -M|--max: let specify max display time

 time is a combination of number+letter where: 
 letter must be: [dhms] 
    d: days 
    h: hours 
    m: minutes 
    s: seconds 

Examples: 
    puppetlast 
    puppetlast -m 1h 
    puppetlast -M 2d 
    puppetlast -M 1h -m 2d 
    puppetlast -M 19h -m 1m 

## Authors

- Esteban M. Navas Martín (algodelinux@gmail.com)
