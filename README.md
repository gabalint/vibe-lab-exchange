<img src="website/logo.svg" alt="OpenBGA Exchange" height="48">

# OpenBGA Exchange: free, open-source interface engine for laboratories

[Presentation website](https://openbga.github.io/exchange/) ·
[OpenBGA Tox](https://github.com/openbga/tox)

OpenBGA Exchange is an open-source project of BGASoft Inc.

**Coming soon.** The first public source release is in preparation. Star or watch
this repository to be notified when it lands.

OpenBGA Exchange is a free, open-source interface engine for clinical
laboratories: the middleware that connects laboratory instruments, LIS/LIMS,
EHRs and other applications. It receives results from analyzers, routes HL7
messages, imports and exports files, and keeps a durable record of every message
it handles. It runs on one computer the laboratory owns, with no cloud service
required.

## What it will do

Planned for the first releases; details may change before publication.

- **Instrument interfaces:** ASTM E1381/E1394 (CLSI LIS01-A2/LIS02-A2) over serial
  and TCP, and vendor-specific analyzer protocols.
- **HL7 v2 interfaces:** orders, results and patient demographics over MLLP, with
  acknowledgements tracked per message.
- **File interfaces:** CSV and other delimited imports and exports, watched folders,
  scheduled pickups.
- **Channels:** a source, optional filters and transformations, and one or more
  destinations, configured without writing code.
- **A durable message store:** every message received and sent, with its
  acknowledgements, retries and explicit failure states, so a transport
  acknowledgement is never mistaken for successful processing.
- **Monitoring:** channel status, message search, resend and reconciliation from
  one dashboard.
- **One computer:** Windows, macOS and Linux. No server to run, no subscription.

## Related project

OpenBGA Exchange is a sibling of [OpenBGA Tox](https://github.com/openbga/tox)
([website](https://openbga.github.io/tox/)), a free, open-source LIS/LIMS for small
US clinical toxicology laboratories. The two are independent: OpenBGA Exchange connects any LIS, LIMS or application that
speaks the supported interfaces.

## License and development disclaimer

Copyright (C) 2026 BGASoft Inc. and OpenBGA contributors. The project's own code,
documentation, synthetic fixtures, website and presentation assets are licensed
under the [GNU Affero General Public License, version 3 only (AGPL-3.0-only)](LICENSE),
unless otherwise identified. Third-party material retains its own terms. Use,
modification and redistribution, including commercial sale, are permitted.
Distributors, and operators who offer a modified version over a network, must
preserve the AGPL rights and provide the corresponding source as
the license requires.

OpenBGA and the OpenBGA product names and logos are trademarks of BGASoft Inc.
The licence does not grant permission to use them (AGPL-3.0 section 7(e)),
except as needed to describe the origin of the software. See [NOTICE](NOTICE).

**This project is vibe coded:** developed with substantial AI assistance and
reasonable effort in research, planning, analysis, review and testing. That effort
does not guarantee correctness, security, regulatory compliance or fitness for
clinical use. The work is provided **as is**, with the warranty disclaimers and
liability limitations in AGPLv3 sections 15–17, subject to applicable law and
written agreements. It is built and tested on synthetic data and is not
clinically validated.
