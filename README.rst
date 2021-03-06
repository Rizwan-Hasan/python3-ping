============
python3-ping
============

A pure python ping implementation using raw sockets.

Note that ICMP messages can only be sent from processes running as root
(in Windows, you must run this script as 'Administrator').

Original Version from `Matthew Dixon Cowles`_

.. _Matthew Dixon Cowles: ftp://ftp.visi.com/users/mdc/ping.py
  
* copyleft 1989-2011 by the python-ping team, see AUTHORS_ for more details.
* license: GNU GPL v2, see LICENSE_ for more details.

.. _AUTHORS: AUTHORS
.. _LICENSE: LICENSE


Usage
=====

::

  ~/python3-ping$ sudo ./ping.py google.com

  PYTHON-PING google.com (209.85.148.99): 55 data bytes
  64 bytes from google.com (209.85.148.99): icmp_seq=0 ttl=54 time=56.2 ms
  64 bytes from google.com (209.85.148.99): icmp_seq=1 ttl=54 time=55.7 ms
  64 bytes from google.com (209.85.148.99): icmp_seq=2 ttl=54 time=55.5 ms

  ----google.com PYTHON PING Statistics----
  3 packets transmitted, 3 packets received, 0.0% packet loss
  round-trip (ms)  min/avg/max = 55.468/55.795/56.232

  ~/python3-ping]# ./ping.py
  usage: ping.py [-h] [-q] [-c COUNT] [-W TIMEOUT] [-s PACKET_SIZE] destination
  ping.py: error: the following arguments are required: destination


TODOs
=====

* refactor ping.py
* add a "suprocess ping", with output parser

New Features
============
* CLI interface -> thanks for Yu-Jie Lin to add this feature with argparse module

Contribute
==========

`Fork this repo`_ on GitHub_ and `send pull requests`_. Thank you.

.. _Fork this repo: http://help.github.com/fork-a-repo/
.. _GitHub: https://github.com/emamirazavi/python3-ping
.. _send pull requests: http://help.github.com/send-pull-requests/


History
=======

See HISTORY.rst_.

.. _HISTORY.rst: HISTORY.rst


Links
=====

* `Sourcecode at GitHub`__
* `Python Package Index`__

__ https://github.com/emamirazavi/python3-ping
__ https://pypi.python.org/pypi/python3-ping
