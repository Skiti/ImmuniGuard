﻿# ImmuniGuard

ImmuniGuard is a mobile app developed as a solution to relay attacks on apps using Google Apple Exposure Notification.
The purpose of ImmuniGuard is to be integrated as a feature in a future release of Immuni app, the Italian contact tracing app.

For each contact with a GAEN-based app user, and specifically an Immuni user, ImmuniGuard locally stores:
* Its own Immuni RPI;
* The other user Immuni RPI;
* Its own GPS coordinates;
* The current timestamp.
This data is merged in a HASH, and stored locally.

Whenever an ImmuniGuard user gets diagnosed with SARS-CoV-2, they can upload all of the HASHES to the ImmuniGuard database.
Other ImmuniGuard users can download those HASHES and compare them with their own.

If the positive user had ImmuniGuard, the HASHES will confirm if other users actually physically met the positive user, or they were victim of a relay attack.
