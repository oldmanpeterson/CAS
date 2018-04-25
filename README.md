# CAS
Config files required for load-balanced CAS setup.
This setup can easily handle the needs of a group of 300 people authenticating from time to time during the day.

Key features include:
  Loadbalancing and failover of loadbalancers
  Active Directory used as the database backend
  CAS configured to be able to communicate to capable applications over the following protocols:
      CAS
      SAML 1,2
      OAUTH
  CAS configured to accept authentication from users using:
      Password form
      Kerberos via SPNEGO
      Google Authenticator tokens for MFA
  CAS attribute resolution (for instance Active Directory group membership) even when SPNEGO auth is used
  CAS Service Management application for more easily creating service definitions

This setup is using:
   Apereo CAS v5.2.2
   Apache Tomcat v8.5.27
   Apache 2.4.6
   CentOS 7.4
   HAProxy 1.5.18
   KeepAlived 1.3.5
   MongoDB 3.6.3

Followed the following tutorial here:  https://dacurry-tns.github.io/deploying-apereo-cas/introduction_overview.html
Gained valuable help from official CAS documentation:  https://apereo.github.io/cas/5.2.x/index.html

The following image a very brief high-level overview:
![alt text](https://raw.githubusercontent.com/oldmanpeterson/CAS/master/cas-high-level.png)
