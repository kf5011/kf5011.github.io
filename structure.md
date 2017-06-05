---
layout: default
---

# Course structure
We have a 12 week semester, with 2 hours of lectures and 2 hours of labs each week.  Based on feedback from the current students I'm going for a 2hour long lab session, and 2 seperate 1 hour lectures.

Having skimmed through [Lee & Varaiya](http://leevaraiya.org/) and [Lee & Seshia](http://leeseshia.org/) I'm thinking there is a good opportunity to make the lectures more theoretical that the previous module.   This would push more into the practical sessions.  There is good scope for putting a lot of directed reading to support both lectures and practicals.

## Some things to Cover
* **Device drivers** Low level access and control of devices, GPIO, configuring
* **Interrupts** Interrupt handlers, timers, rising/falling edge buttons
* **TCP/IP stack, OSI model** physical layer, link layer, and application layer
* **Data formats** YAML, JSON, XML
* **Data logging websites** api, data analytics
* **Digital Signals**
* **Analog Signals**
* **Sampling** Nyquist limit

## first go at a  weekly plan
A first cut at some structure.  Based on existing module,

It may want some revision in the light of Lee & Varaiya, and Lee & Seshia.

|     |theme | Lecture  | Practical   | Lecture  | Practical |
| --- | -- | --  |-- |
|1 |  | | | | |
|2 | digital | Interface Arch | Digital in | Interface devices and circuits | Out
|3 | analogue | Analog sensors & interfacing | Analogue input |
|4 | interrupts | Interrupt handling | timers | | buttons |
|5 | busses SPI, I²C|  | Control loops | feedback exercise
|6 | Serial | Serial comms to PC | HCI | PC interface
|  | assignment 1 | builds from practicals
|7 |Data | Data logging | sample | Network stack, terms DNS, IP, MAC, UDP rfc1122/rfc1123 rfc768|
|8 |     | Data formats, text, XML, Json, Yaml | parsing text | Application layer HTTP rfc2616/rfc7540, POP rfc1123  | Log data to server
|9 | Control | Commands, formats | Protocols |  Remote Control
|10|Security | Authentication, validity, md5 hashes, sha/NIST FIPS 180-4| | TLS rfc5246, SSH / HTTPS rfc2818 |
|11|Encryption | | PGP/ rfc4880
|12|
