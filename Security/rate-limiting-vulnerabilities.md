#Rate limiting vulnerabilities

**Affected Versions**

Meteor < 1.2

**Expected Solutions**

Meteor 1.2+

**Workarounds**

[Sikka - A Firewall for Meteor Apps](https://github.com/meteorhacks/sikka)

##Description
DDP vulnerabilities can exist if there is no prevention strategy against rate limiting of simultaneous connections to prevent for example brute force attacks. Such vulnerabilities can lead to denial of service.

##Related Sources
[Rate limiting in Meteor core](http://info.meteor.com/blog/rate-limiting-in-meteor-core) from Meteor
