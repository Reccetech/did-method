# Argumentation around budgetting
## Connections and sharing

The scope changed slightly for the core functionality of Connections and Sharing:
* Added deeplink functionality for connnection invites
* Added one step connect and share
* Added extra extra security mitigation to update the connection with the identity of the invitee


## Basic Vault (+ SSO Flow)
The basic vault is new functionality on request of KBC compared to the original quote of April 2021.
The orgininal scope was limited to share and connect between plus account holders.
The basic vault is a limited version of a normal vault:

Alternative to the basic vault was the read-only vault. However, during our feasbility analysis we budgetted that the read-only vault has a 50% higher costprice compared to the basic vault, due to a number of complex edge cases that can arise in downgrading a vault from normal to basic.

## Notifications 

This is additional scope from KBC to offer the end-user direct feedback on certain events that happened inside their vault:
* Accepted a connection
* Rejected a connection
* Revoked a connection 
* Received a share
* Updated a share
* Revoked a share

We budgetted an extra service that will run as background process to dispatch the message to the correct KBC Vault user when a certain is triggered. 

We also introduced in-app notifications to offer more context to the end-user and offer the posibility to include action based on this context.
The latter part can be seen as optional scope, which was asked in context of a better and friendlier UX experience. 