 # Authentication

 **What is OAuth?**

 OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

 **Give an example of what using OAuth would look like.**

When you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon.


 **How does OAuth work?**
  
  The first website, which provides the confirmed user identity, links the second website on behalf of a user using OAuth. The second website produces a single token and a unique secret for all parties engaged in the transaction. This token and secret is provided on the initial site to the client software of the beginning user.

 The customer software offers its authorization provider the token and secret (which may or may not be the second site).

 If the authorization provider is not already authenticated, the client might be requested to authenticate. The customer is requested to authorise the authorisation transaction to the second website after authentication. A certain sort of transaction on the first website is approved by the user (or its program quietly authorizes). A token is issued for the user (note that it is not a request token anymore). The user provides the first website with the allowed access token.

 As evidence of an authentication for the user, the first website provides the access token to the second website.

 On behalf of the user the second website provides access to your site. The user sees a transaction successfully completed. The OAuth system is not the first to operate in this fashion on behalf of the end user. Actually, many authentication systems function similarly, especially Kerberos. OAuth's ability to work the whole internet and its broad acceptance is exceptional. Adoption rates were successful when prior efforts failed (for various reasons).


 **What is OpenID?** 
  >OpenID is an open standard and decentralized authentication protocol. Promoted by the non-profit OpenID Foundation, it allows users to be authenticated by co-operating sites (known as relying parties, or RP) using a third-party service, eliminating the need for webmasters to provide their own ad hoc login systems, and allowing users to log into multiple unrelated websites without having to have a separate identity and password for each. Users create accounts by selecting an OpenID identity provider and then use those accounts to sign onto any website that accepts OpenID authentication. Several large organizations either issue or accept OpenIDs on their websites.


