---
layout: single
title:  aSocial project description
date:   2021-01-30 20:00:00 -0700
categories: project asocial distributed network encryption
---
Hello dear reader,

The aSocial project was started quite a long time ago (~28.12.2013) when I combined my thoughts
about the distributed social system and Bitcoin network to fix the spam issue. Unfortunately the new
projects forced me to put this one into desk, but I think the time has finally come to rethink it
from scratch and drive forward. And here I will describe what kind of ideas is in the project and
what is the base for it.

{:refdef: style="text-align: center;"}
[![aSocial logo](/assets/images/blog/2021-01-30/asocial_logo.png)](/assets/images/blog/2021-01-30/asocial_logo.png)
{:refdef}

**aSocial**: "Share your data with the ones you trust the most"

# Rough Summary

The modern world is a collection of centralized social networks and instant messengers which are
happy to own your social information without any restrictions on its actual use. This project was
created to solve the unpleasant problems of centralizing the storage of important information, fight
censorship, simplify communication and interaction of people, and also protect them from outside
encroachments.

[![aSocial UI main](/assets/images/blog/2021-01-30/asocial_ui_main.png)](/assets/images/blog/2021-01-30/asocial_ui_main.png)

**aSocial** - is a distributed, private and secure social network for those who care about freedom
of communication and want the complete control over their social information. It will allow you to
interact using secure communication channels, store your memory of generations on your controlled
devices, fight useless information through paying for its reception, simplify the search for new
acquaintances and open up opportunities for building reliable and secure social applications.

Naturally, the source code will be completely open to the public - nowadays it is impossible to
trust closed products and closed algorithms with which they handle our data. The platform will be
based on the p2p communication technologies, in which there is no central server - which improves
security and censorship resistance to a level unattainable for modern communication systems. It will
open up the opportunity for information monetization using Bitcoin & Lightning networks, pave the
way for simplifying interfaces, remove difficulties and worries in the distribution of content,
unify and protect the storage and processing of social information, allow flexible interaction with
history - in general, it will give full control over what, how and when it happened, is happening
and will happen in your life, the lives of your friends, relatives and other social agents.

# 1. Project overview

## 1.1. Purpose

The main goal of the project is to create a distributed and secure platform for user interaction in
any form without restrictions.

Freedom and privacy of interaction are the most valuable good for the individual and it should be
strived for, and it cannot be subject to any restrictions. Even if this communication may seem
"harmful" to someone, this is only a private judgment and everyone is free to choose their own
destiny in connection with the circle of their communication.

The system must also be sufficiently secure to also provide the ability to deny the interaction,
since this is a personal choice of the individual - to disclose any personal information or not,
we live in an imperfect world in which many threats depend on information received by criminals.

## 1.2. Scope

In general, aSocial should become the most widespread system for interaction and storage of social
information, breaking down barriers between people and simplifying communication and processing of
such data, including freeing society from excessive centralization.

## 1.3. Core features

In order to build a better social system, you need to think about the main features in which I can
include:

* **Modularity** - you can add or throw out not important system components (UI - native, WEB,
console) or replace important ones with analogs (databases, for example). This will allow the system
to be deployed on servers or wearable devices while meeting the specified security and
responsiveness requirements.

* **History** - is not only the ability to create elements (events, agents ...) at the right times,
but also to observe their changes over time. For example, changing your friend's last name is
important information, incl. the opportunity to see how it was before the change is no less
important.
   * End-to-end change history with the ability to rewind
   * Timeline is a convenient display of events and areas of life (lived / worked) for agents
   * Grouping and tagging changes

* **Persons** - are basically profiles of people or organizations with whom we interact in society.
They may not have a profile, but exist as your (or collective) memory of them. You can leave your
vision about any person.
   * A profile can have several persons for different tasks, for example “Friends”, “Work”,
   “Relationships” and any others. A separate address is generated for these and are used as a
   starting point for communication.
   * Each profile has a pair of keys, which is used to generate invite keys so can form a tree of
   connections and you can work with information in terms of leaves or branches or the whole tree.

* **Events** - "what happens", usually has a beginning and sometimes an end, like the current place
of residence, work, school, party, or when you find something important.

* **Messages** - both communicating with other agents and requesting profile updates (which occur
mainly in the background).
   * Tied to monetization to solve the spam problem.
   * Thread tree with the ability to transfer messages
   * Title / description / tags of branches
   * Easy import from other messengers / social networks
   * Update request (news from the media, for example)

* **Overlays** - are an opportunity to have your own opinion on any information you've got. They can
be protected (password) or unprotected, optional (enabled and disabled as needed) and associated
with certain base objects or creating new objects. For example, you can add a friend to your
network, even if he does not have a profile, and later, if he is added, link his profile. Or, in the
overlay, you can change its name to an alternative one.

* **Synchronization** - you own several devices and these devices can sync profiles between each
other and perform different roles, for example, you can fumble your favorite collection of movies
from the desktop, but still not have them on your phone.

* **Sharing** - needed for transferring multimedia and other files. Uses bittorrent for upload and
download.

## 1.4. Additional features

On the basis of the basic capabilities, additional functionality will be made (or even follows):

* **Tree of life** - each of us has a generational history that we want to pass on to our children,
so why not on the same social network? This is a convenient display of family ties between persons.

* **Wills** - are a type of stored messages and the ability to set conditions for activating their
sending or destruction. Free on controlled devices and paid on relays. For example, being offline
for a month triggers the distribution of these messages.

* **Contracts** - are messages in which you agree to certain obligations. These obligations are
signed by both parties, they can block certain funds for a certain period, etc.

* **Web interface** - is a module with which you can access your profile remotely using HTTP, you
just need to launch the application, enable the module in the settings and open the desired host and
port in the browser.

* **Consensus** - is an addition to group chats to quickly resolve issues of agreement with a group
of people. If the person agrees with the proposal, then one vote is added. If not, he opens a
discussion to find a compromise among all participants. A decision is made as soon as each member of
the group agrees.

# 2. Obstacles

## 2.1. General

The development of aSocial will cause the following problems:

* Most likely, it will be too difficult on my own - I can miss important points and miscalculate in
the main ideas, therefore peer-review and discussion of concepts are necessary in the early stages
of building the system. For this, this document exists - to immerse potential associates in the
problem and identify missed moments in order to continue interaction in the future and jointly bring
the system to a ready state.

The adoption of the new social network by users will face obvious challenges:

* User suspicion - anything new naturally raises questions, especially so many innovations. Again,
the openness of the project can in general terms solve the question of suspicion - but you will
probably have to make additional efforts to show and tell.

* Resistance from politicians - they will try to put a spoke in the wheel because of the
conservatism and the complexity of managing a decentralized system. Also, lobbying large
corporations (Facebook) may have an impact on overall development. The path of bitcoin in this
regard seems to be reasonable - users will choose a more convenient system no matter what.

* Counteraction of intelligence services - they always want to get into user communications under
the guise of fighting terrorism, which is obvious nonsense. They will try to embed backdoors under
the guise of useful functions, but I think that the open nature of the platform, community auditing
and the lack of centralized management neutralize this risk to a minimum.

## 2.2. Technical

Such distributed systems require special care in the development of the interaction protocol, since
it will be quite problematic to change it.

# 3. Industry and Market Risks

Social networks and messengers (these areas are the focus of this development), so entry to the
market is initially based on stakeholders (geeks, programmers, security professionals), from where
it may well spread further if convenient means of interaction are available.

# 4. Budgetary Risks

Development is driven by pure enthusiasm, so budgetary risks are irrelevant, at least during the POC
development stage. As soon as the budget appears, they will need to be revised.

# 5. Hardware

Target platforms for application launch:

* Android - most phones and wearable devices in the world
* Linux - open source and all servers on the Internet
* Windows is still the majority of workstations and hamsters
* MacOS - working systems with UI, gradually superseding Windows
* iPhone - Possibly, but most likely last due to the complexity of the ecosystem.

Separate hardware is not required, but the battery and communication capabilities between devices
will need to be considered.

# 6. Software

## 6.1. Architecture

As the main platform is used by Qt5 with add-ons for each platform, the application is divided into
two modules - backend and frontend:

### Backend

It deals with background activity - interacts with devices nearby and via the Internet, transmits
and receives data from other devices (for example, someone else's encrypted messages for further
transmission), receives updates. Stores intermediate already encrypted data in LevelDB.

### Frontend

User interface for managing profiles. Main storage is SQLCipher (SQLite with encryption).

## 6.2. Storage

For storage, a pair of local databases is used - the built-in unencrypted nosql storage LevelDB,
which is necessary to maintain the data transfer service, and the encrypted sql storage SqlCipher
(add-on over sqlite3) for storing profile data.

### LevelDB

It allows you to store key-value data that is not valuable for a potential attack - these are
connection lists, encrypted relay data... In general, the data that are necessary for interaction
between systems in hibernation mode. Also stores password-encrypted keys from available profiles.

### SqlCipher

An encrypted database for storing important profile information. It is decrypted in chunks as needed
using a long key.

### File storage

The described databases are stored on the local file system.

Regular files and media are stored unencrypted on the file system. Individual photos / videos can be
encrypted directly at the file level if necessary and will be available exclusively from aSocial,
since all known operating systems do not support decryption mechanisms at the file level.

## 6.3. Communication

The profile is a set of data encrypted with a cryptographic key, encrypted with a password.

When initializing a connection with another profile (social agent), a unique key for communication
is created - i.e. any communication with the outside world is carried out on a unique pair of keys
to prevent problems of reusing the same key. This key can only be used by those who received it. You
can also connect additional keys to the profile (or generate them) - they can be used to initialize
new connections, distribute your profile or receive donations / single messages.

Trying to find other people are, in any case, publishing information, but not necessarily the one
that is posted on your profile: you can create a separate layer in which you can add information of
your choice so that other people can find you.

During communication, any available means are used - Internet, Mesh, WiFi-direct, Bluetooth, NFC,
USB-dongle ... As an interaction protocol, you need to examine the available open source libraries
for messengers. They already support e2e encryption, chats, NAT-traversal and can be useful
initially.

## 6.4. Security

Security is the starting point of this project. It is not only about encryption, but also the
confidence in complete control over the information you own. Any permissions to provide information
to the outside are completely controlled by the user using filters and privacy levels (implemented
as overlays / layers), which are switched using different passwords and encrypted with different
keys.

I think everyone wants to appear a lot better for other people than they are - and we see that social
media profiles are mostly pretentious perfect. But modern social networks mostly forget that there
are those very real people behind a beautiful picture who are unable to store their data somewhere
other than their own heads. aSocial will improve this system and allow you to store and share with
certain people even confidential and secret information.

Thus, aSocial allows you to create different public identities or different faces can be implemented
using different profiles that can coexist on the same device. The base level of the profile is your
public identity.

When creating a profile for overlays, a randomly sized encrypted space is initialized. This space is
used for placing more secret information on an onion principle (each subsequent level can be opened
from the previous one with a unique password). Thus, any user can deny the very existence of
additional levels.

Initially, the platform supports full traffic encryption, end-to-end encryption of messages, the
possibility of plausible denial of any action or the presence of a profile at all. Built-in it is
possible to choose an encryption system, depending on the secrecy of the message:

* **Normal** - durable and compact, different types can be selected. Size is the compressed original
message.

* **Ambiguous** - the ability to send two different messages in a single message, which can be
selected depending on the specified key. The encrypted messages are shuffled and the sampling
algorithm depends on the data in the key.

* **Shuffled with a random message** - is a kind of ambiguous, necessary in order to help other
people with ambiguous encryption. The second key is not disclosed, and the data for the second
message is generated randomly. Size - ~ 2x compressed original message. This is the default to
improve the security of the entire system.

* **Probabilistic** - a very large message size, just as an additional option for geeks - they are
geeks and know what to use it for :)

(ambiguous encryption mixed with garbage, or probabilistic encryption, which implies an increased
cost per message due to its increased size).

## 6.5. Spam, Ad & Monetization

The need to include the payment system in the social network is dictated by modern realities.
Firstly, it allows you to fight spam and advertising, and secondly, it is an opportunity to create
a new platform for the monetization of information and its distribution.

The main problem of spam and advertising is distraction, they literally gobble up our time, thus we
pay our most expensive resource for someone else's and mostly useless for most product promotion.
Remember incoming SMS on GSM networks - they are distracting, advertising on the Internet is
insanely distracting. Based on this, we must fight against such harmful phenomena, and the best way
to fight is to increase the payment for displaying the message. Thus, the user has the opportunity
to restrict the circle of persons, while not completely blocking messages from the outside.

In aSocial, you can set the board to receive messages of several levels depending on the value of
the communication frequency. Thus, you will receive a fee and after that a message appears; if the
fee is less than the minimum, it is ignored. The importance of the message is selected depending on
the level of payment:

* Minimal - the message appears in the message list, there is no user notification. Used for
subsequent messages in an active conversation.

* Medium - additional to the minimum - normal pop-up window with a notification about the arrival of
a message. It is used by default for the first message of a new conversation or for continuing a
conversation after a long time.

* Promoted - important messages with a special pop-up window and continuous notification that does
not stop until the message is read.

Billing depends on the size of the message - a larger message will take longer to read.

A request (update) of information may also require payment - for example, a public figure or the
media may demand a payment for receiving public information about him / the latest news.

The technology used is Bitcoin (like the Lightning network). When you add a new contact, you set up
a new Lightning channel for exchanging funds - and they are sent back and forth when you exchange
messages. First, you receive a message and a transaction ID sent to the Bitcoin network to initiate
a lightning microtransaction channel. You receive it (if the funds sent are sufficient) and continue
communicating via the open lightning channel or close it and collect the funds received. In fact,
messages are sent along with the contract for the transfer of payment, so before distracting you -
aSocial will check the validity of the transaction.

When using relays (sending and temporary storage of a message - for example, due to the
inaccessibility of direct communication with the recipient), you additionally pay for the reception
and storage before sending it to the relay operator. In mesh networks (based on bluetooth / wifi and
other short-range communication systems), users can also charge a small fee for sending / storing a
message - but by default such a relationship is free, but it is regulated by the cache size, the
budget for application activity and the device charge (to regulate battery consumption and other
resources).

For example, you are a world famous creator of the Linux kernel, your time is insanely expensive -
and you have the right to set a fee for incoming messages: for close friends with whom you often
communicate - the fee may be close to zero, for outside unknowns - the fee is set depending on your
requirements.

A good cost guideline is your hourly salary (distraction for an hour) multiplied by 2..4 (because
it's a personal time). With your hourly payment of $20, the cost of a message from a stranger will
be priced ~$40-$60 (~1mBTC with 1BTC = $34000) seems quite reasonable. I would read a spam message
for $60 - no question at all ;)

# 7. Predecessors

Multiple social networks and messengers have already been created in the world with varying degrees
of security, decentralization, convenience - so you need to understand on what foundation this
development begins. Here are a few major development milestones:

## 7.1. Centralized

### IRC / ICQ / Jabber

It all started with IM and chats, as people wanted to communicate. They allow you to exchange
messages, links, participate in discussions and store history, but they are very limited in
transferring your Self to the virtual space, i.e. not suitable for storing social information.
They have their own user database and are mostly centralized or federated.

### Facebook / Vk

The first popular social networks in the full sense of the word. They stood out for their ease of
use and the absence of a separate client (WEB-interface). Allowed to more or less conveniently
search for classmates and friends (allowed to create a profile with a good life description), as
well as share content with them in the form of a wall on your personal page - and this has gained
immense popularity among users.

Their main problem was centralization - this is a huge pot of honey (like any more or less large
database), attracting insiders and hackers. They also do not support p2p encryption, are saturated
with ads and sell / distribute your information to the right and left. I think today it is already
obvious that trusting your information for free is not only useless, but also harmful. The benefit
to the end user is negligible, and the damage received (from ads, leaks, errors, blocking,
censorship) is much greater.

### Twitter / Instagram / Youtube

Highly specialized, centralized social networks that have taken over all the shortcomings of their
older brothers.

### Skype / WhatsApp / Telegram / Signal / Wire / Slack

Active messengers that do their job pretty well, which are mainly aimed not at some semblance of
privacy, although they are still centralized in nature and focused on “not storing” classified
information (secret chats), which generally negates their usefulness.

## 7.2. Distributed

Unfortunately, [the majority of distributed social networks](https://en.wikipedia.org/wiki/Comparison_of_software_and_protocols_for_distributed_social_networking)
are somehow written in web-based languages, which imply client-server interaction and undermine the
very essence of distribution. These are usually complex to install, requiring databases and
non-trivial skills to maintain. Others are heavily outdated, investor-controlled or in their
infancy...

### RetroShare

Good, but drawn-out development of a decentralized messenger. Interesting developments in
decentralized communication using DHT, tor / i2p and NAT-piercing, which can be adapted to work in
aSocial. Disadvantages as a messenger include:

* Poor support for mobile devices - In today's world, it is difficult to imagine an application that
is not natively focused on wearable devices.
* Morally outdated interface shipping in 2000
* It looks more like an attempt to combine disparate technologies for user convenience, rather than
an attempt to rethink communication.

### Diaspora / Matrix (and other server-based)

It is aimed at combating centralization rather than user security and privacy. The concept of pods
implies a half-measure - your information is still owned by someone other than you. Of course, you
can raise your pod - but this is a very non-trivial task.

### OpenBazaar

Those who got close enough to decentralization and anonymity, but deviated from their original
ideas, the project of an open market and replacement for ebay / amazon marketplaces. He successfully
uses Bitcoin for settlements, but caved in under pressure from investors and turned off the built-in
anonymity functionality.

# Conclusion

Overall the aSocial project should be the huge win for everyone, so soon I will prepare the project
page and share the rewritten build system to start it again.
