# BSIM

A Bitcoin Secured Instant Messaging Protocol

## Purpose

This protocol aims at creating a set of rules for an Peer-to-Peer Instant Message exchange system secured by Bitcoin transactions.

## Mechanisms

### Account creation

An account is just a Bitcoin Address that has a locking vOut.
The amount and the time-lock period is chosen by the person creating it.

#### 1 - Search for a contact

To initiate a chat one must find the Onion Address related to the Bitcoin Address of the contact. This is done searching a DHT.
If any peer has the Onion Address from this account you can initiate the chat directly to the contact.

#### 2 - Checking minimum lock

The client has to check that the amount time-locked by the peer initiating the chat satisfies the minimums set in the client.
If this check is positive, the chat can be initialized.

### Secure Messages

All the messages use a Public - Private Key Cryptography. The user sending the message encodes it using the other peer Public Key. The user receiving the message can decode it using it's Private Key.

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/ipms-io/bsim/tags).

## Authors

* **Níckolas Goline** - *Initial work* - [nGoline](https://github.com/nGoline)

See also the list of [contributors](https://github.com/ipms-io/bsim/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
