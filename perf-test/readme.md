jmeter `5.0`

the first test runs against the documentation, the second views three pages of a TEI document from TEI Publisher.

Apps are the current ones available in public repo.

In both cases increased -Xmx to 4096m, but otherwise left eXist unchanged.

Test | Version | AVG | MAX | Threads
-----|---------|-----|-----|--------
status-docs.jmx | 4.x.x | 257 | 2713 | 30
status-tei.jmx | 4.x.x | 643 | 5565 | 20
status-docs.jmx | develop | 2587 | 24261 | 30
status-tei.jmx | develop | 3946 | 21765 | 20
