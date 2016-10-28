# OSDFCon2016
Place holder for OSDFCon 2016 Presentation

## Event Logs
In the presentation we covered Event Log nexted data. We parse EVTX using [EventMonkey](https://github.com/devgc/EventMonkey). The report templates used can be found here [https://github.com/devgc/EventMonkey/tree/master/sqlite_templates](https://github.com/devgc/EventMonkey/tree/master/sqlite_templates)

## Link Files
For link parsing we used [GcLinkParser](https://github.com/devgc/GcLinkParser) to output into a SQLite database. The SQLite templates can be found here [https://github.com/devgc/GcLinkParser/tree/master/sqlite_templates](https://github.com/devgc/GcLinkParser/tree/master/sqlite_templates).

## Connecting Link and ShellBags
For shellbags parsing we used Eric Zimmerman's [SBECmd.exe](https://ericzimmerman.github.io/) which is found within Shell Bag Explore package. Out put was to TSV. The report was then added to the link files SQLite database with table name 'sbags'. A query can now join the previous sqlite template to get path references and the shellbags file entry, sequence, and folder name.
