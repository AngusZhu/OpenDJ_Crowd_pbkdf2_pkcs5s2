OpenDJ_Crowd_pbkdf2_pkcs5s2
===========================

The original java class file comes from the OpenDJ repository, see:

http://sources.forgerock.org/browse/opendj/trunk/opends/src/server/org/opends/server/extensions/PBKDF2PasswordStorageScheme.java?hb=true

and adapted to follow Crowd (and all the Atlassian products) and ApacheDS implementation of the PKCS5S2 password encoding hashing, see:

http://pythonhosted.org/passlib/lib/passlib.hash.atlassian_pbkdf2_sha1.html

https://issues.apache.org/jira/browse/DIRSERVER-1898

# Changes

The implementation differs of:
 * increased salt size to 16 bytes
 * increased hash size to 32 byes
 * modified the prefix to {PKCS5S}
 * the salt prepended to the hash
 * convertion to utf-8 of the password in plain text

The difference left is the number of iterations printed after the prefix 
