# PAGASA Parser
The PAGASA Parser project is a volunteer-run effort to provide parsers and archivers in an attempt to make Philippine Atmospheric, Geophysical and Astronomical Serivces Adminstration (PAGASA) Tropical Cyclone Bulletins (TCB) machine-readable and usable.

This project is volunteer-driven and not affiliated with the PAGASA.

## Web interface
The best way to use the PAGASA Parser is through its web interface at https://pagasa.chlod.net. Here, you may parse bulletins that are currently on the PAGASA file repository. Optionally, you can run the PAGASA Parser web interface locally using [this Docker image](https://hub.docker.com/r/chlod/pagasa-parser-web/).

This website is run for free. Donations for alleviating server costs are appreciated.

## Packages
The following packages are available for use.

### pagasa-parser
| Package | Repository | Details | Description |
|---|---|---|---|
| pagasa-parser | [link](https://github.com/pagasa-parser/pagasa-parser) | [![npm version](https://img.shields.io/npm/v/pagasa-parser.svg?style=flat-square)](https://www.npmjs.org/package/pagasa-parser) | Core package. Required by other packages. Extracts area strings and does general text parsing. |
| @pagasa-parser/source-pdf | [link](https://github.com/pagasa-parser/@pagasa-parser/source-pdf) | [![npm version](https://img.shields.io/npm/v/@pagasa-parser/source-pdf.svg?style=flat-square)](https://www.npmjs.org/package/@pagasa-parser/source-pdf) | Reads PDF bulletins. |
| @pagasa-parser/source-xml | [link](https://github.com/pagasa-parser/@pagasa-parser/source-xml) | [![npm version](https://img.shields.io/npm/v/@pagasa-parser/source-xml.svg?style=flat-square)](https://www.npmjs.org/package/@pagasa-parser/source-xml) | Reads a special XML format. Mostly used for "parsing" custom bulletins. |
| @pagasa-parser/formatter-signals | [link](https://github.com/pagasa-parser/@pagasa-parser/formatter-signals) | [![npm version](https://img.shields.io/npm/v/@pagasa-parser/formatter-signals.svg?style=flat-square)](https://www.npmjs.org/package/@pagasa-parser/formatter-signals) | Transforms a parsed bulletin into a map, where municipalities and provinces are colored by storm signal. |
| @pagasa-parser/formatter-wikipedia | [link](https://github.com/pagasa-parser/@pagasa-parser/formatter-wikipedia) | [![npm version](https://img.shields.io/npm/v/@pagasa-parser/formatter-wikipedia.svg?style=flat-square)](https://www.npmjs.org/package/@pagasa-parser/formatter-wikipedia) | Transforms a parsed bulletin into a Wikipedia {{[TyphoonWarningsTable](https://en.wikipedia.org/wiki/Template:TyphoonWarningsTable)}}. |

### pagasa-archiver
This project also handles the [pagasa-archiver](https://github.com/pagasa-parser/pagasa-archiver), a tool for scraping and downloading bulletins from the PAGASA files website for archiving. Usage instructions can be found on its repository.

For a live list of archives, you can check [User:Zoomiebot/Archives/PAGASA](https://en.wikipedia.org/wiki/User:Zoomiebot/Archives/PAGASA) on Wikipedia.