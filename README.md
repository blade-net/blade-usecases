# Blade Use Cases

The following use cases have been defined for the Blade ecosystem to highlight the benefits and advantages over other approaches for decentralized service ecosystems.

## Preamble

For the use cases defined in this document, we consider three users, Alice (A), Bob (B), and Charlie (C). Each user owns a Blade server S(X) for user X and accesses its functionality via a Blade client Cl(X). Users are identified via an Ethereum address Id(X), which is derived from the keypair IdKey(X). Furthermore, each user has a delegate keypair DelKey(X).

## Use Case 1: Installation and Identity Creation

Alice wants to host her own Blade server S(A) on a device in her home network. She downloads the latest version of the project and installs it. Using the administration panel, she creates a local user account which she will use to login to her own Blade server instance to access its functionality. During the registration process, two cryptographic keypairs are automatically created: her identity key pair IdKey(A) and a delegate key pair DelKey(A).

In order to connect to and communicate with other users in the Blade ecosystem, Alice needs to register and create a decentralized identity in the Blade registry.
Using the administration interface of her Blade server, she registers an identity with the Blade registry, which is created using her identity key pair IdKey(A).
In this process, her identifier Id(A), which is derived from IdKey(A) is registered in the registry and stored together with her delegate key pair as well as the network location (i.e. URL or IP address) of the S(A).

During the registration, Alice also registers a globally unique username Name(A), which allows resolving to both her identifier and associated information. This identifier is preferably human readable and can therefore be used to exchange identifiers in a non-technical setting.

## Use Case 2: Connection

Alice wants to communicate with her friend Bob using an instant messenger service she installed on her Blade server S(A).
She logs in into her Blade server and uses the search functionality to look for users called Bob, which returns a list of 5 different users named Bob.
Each user is described with a profile picture and a short textual description, allowing Alice to easily select her friend from the list and send a connection request to him.
The connection request is digitally signed using Alice's delegate key pair DelKey(A).

The connection request is received by Bob's Blade server S(B) and stored for later review by Bob.
The next time Bob logs in on his Blade server, he is notified about the new connection request from Alice.
Once he accepts the request, a response message is sent back to Alice informing her about his decision.
To also add Alice also to his own contact list, Bob sends a similar connection request to Alice.

## Use Case 3: Marketplace & Module Installation

TBD

## Use Case 4: Module Development

TBD
