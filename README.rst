show_my_ip.py
=============

There is no ``ifconfig`` in Cygwin,
so I wrote a little Python script to parse the result of ``ipconfig`` to get the name of NIC cards and their IP addresses.

The encoding of ``ipconfig`` is ``CP950``, I decoded it and encode it again with ``UTF-8``.

The function in the script returns a dictionary, with key as name and value as IP address.
