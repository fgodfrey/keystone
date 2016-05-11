==================
OpenStack Keystone LDAP Cache
==================

This repository is a fork of the real OpenStack Keystone repo.  Please check that repo out if you are looking for official code.

This repository contains the liberty-ldap-cache branch, which is branched from stable/liberty for the purposes of implementing an LDAP cache.  This cache is somewhat basic and assumes that, other than authentication, once an LDAP record is known, it won't change (or be deleted).  So, obviously, there's a lot to improve.

The purpose of implementing this cache is to improve latency of requests to Keystone in environments that use read-only-LDAP.
