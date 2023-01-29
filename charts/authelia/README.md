# authelia
This is a highly opinionated, cut-down version of Authelia that is intended for use by a handful of users in a home lab environment.
This chart specifically makes the following choices with the subsequent limitations:

 - User database is mounted via a ConfigMap, therefore password reset is disabled
 - Session storage is ephemeral; restarting pods causes session to disappear
 - No notifications setup

Any of the above can be changed by overriding `authelia` chart values. See [the official authelia chart](https://github.com/authelia/chartrepo/tree/master/charts/authelia).
