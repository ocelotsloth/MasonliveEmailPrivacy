# MasonliveEmailPrivacy

## Motivation

George Mason University recently began implementing a "security" regime which
threatens the safety of the thousands of users who use their email hosting for
academic communication.

This technology, called "URL Rewriting," involves modifying the links sent to
student email accounts to pass them through a link reputation checker. While a
good idea, the service then stores all of the activity in a database for later
lookup in case a new website is found. This breach of user privacy was not
properly explained, and GMU ITS provides no mechanism to opt out of this
program.

## Solution

This repository is going to host several different utilities which together
will be able to reduce the impact that this program has on user privacy.

### Plain-text MUAs

For users who use plain-text mail readers such as Neomutt, a script will be
provided to pass all email through which will convert the tracked links back
to their unfiltered state.

### Web-Based Email

Once the Plain-text filter is finished development will begin on a universal
browser extension which will be capable of undoing the link-rewriting so that
users of webmail will be protected.

### Host-Based Redirection

The most aggresive solution, this utility will act as a proxy to the proxy
service which can be self-hosted and protect users from this program. A
free-to-use instance (with no logging) will be setup to provide redirection
for less-technical users who want this service.

