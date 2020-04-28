..  MusicBrainz Picard Documentation Project
..  Copyright (C) 2020  Bob Swift (rdswift).
..  Permission is granted to copy, distribute and/or modify this document
..  under the terms of the GNU Free Documentation License, Version 1.3
..  or any later version published by the Free Software Foundation;
..  with no Invariant Sections, no Front-Cover Texts, and no Back-Cover Texts.
..  A copy of the license is available at https://www.gnu.org/licenses/fdl-1.3.html.

$endswith
=========

| Usage: **$endswith(text,suffix)**
| Category: conditional
| Implemented: Picard 1.4

**Description:**

Returns true if ``text`` ends with ``suffix``.  Note that the comparison is case-sensitive.


**Example:**

The statements below return the values indicated::

    $endswith(The time is now,is now)  ==>  "1"  (True)
    $endswith(The time is now,is NOW)  ==>  ""   (False)
    $endswith(The time is now,)        ==>  "1"  (True)
    $endswith(,)                       ==>  "1"  (True)
    $endswith(,now)                    ==>  ""   (False)