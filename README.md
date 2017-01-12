puppetlast
==========

Overview
--------

This program shows the last connect time of puppet nodes.  
It currently displays them in green if they've connected in seconds or minutes.  
It currently displays them in red if they've connected in hours or days.  

Installing
----------

You can install it simply running these commands on your puppetmaster::

   $ wget --no-check-certificate -O /usr/local/sbin/puppetlast https://github.com/algodelinux/puppetlast/raw/master/puppetlast  
   $ chmod 755 /usr/local/sbin/puppetlast 


## Authors

- Esteban M. Navas Martín (algodelinux@gmail.com)
