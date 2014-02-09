OpenDJ_Crowd_pbkdf2_pkcs5s2
===========================

This java class file has been take from the OpenDJ repository, see:

http://sources.forgerock.org/browse/opendj/trunk/opends/src/server/org/opends/server/extensions/PBKDF2PasswordStorageScheme.java?hb=true

and adapted to follow Jira and ApacheDS implementation, see:

https://issues.apache.org/jira/browse/DIRSERVER-1898

# Changes

The implementation differs of:
 * salt size
 * hash size
 * salt prepended to the hash
 * convertion to utf-8
