Describe how you would configure, secure, and monitor tls configuration for a web site and tech stack of your choosing. At minimum your stack should have an ingress, application, and database running.

We are looking for
* automating the TLS issuing, and how its done (http vs dns challenge)
    * can be aws acm, k8s cert-manager, service mesh, cert bot, even heroku if they are inclined.
* tls versions used
* monitoring tls cert expiration and validity
* tls used for db connection
* end to end tls from client to db
* no downtime
