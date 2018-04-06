# AMWA NMOS Parameters Repository

The [AMWA Networked Media Open Specifications](https://github.com/AMWA-TV/nmos) are intended to support extensibility, using constants for parameter values that identify additional operational constraints or capabilities. In order to promote interoperability, this repository contains entries for constants used, for example, with the [Discovery and Registration (IS-04)](https://github.com/AMWA-TV/nmos-discovery-registration) and [Device Connection Management (IS-05)](https://github.com/AMWA-TV/nmos-device-connection-management) Specifications. These specifications do not require values to be included in this repository but doing so allows common definitions to be shared and deployed more easily.

Parameter values recorded herein may be applicable to one or more of the AMWA NMOS specifications, and to one or more versions of each specification. The Parameters Repository as a whole is not versioned, and is expected to be updated as needed to promote interoperability.

## Parameter Repositories

The following parameter repositories are maintained:

- [NMOS Node Service Types](node-service-types/)
- [NMOS Device Control Types](device-control-types/)
- [NMOS Formats](formats/)
- [NMOS Transports](transports/)
- [NMOS Device Types](device-types/)

Each parameter repository provides guidance and considerations for when and how values can be included, and identifies the procedures for revision and deprecation of entries.

New parameter repositories may be added in the future as required by AMWA NMOS specifications.

### Parameter Repository Guidance

The [NMOS Node Service Types](node-service-types/) parameter repository provides a typical example. IS-04, since v1.1, allows a list of 'services' to be advertised on the node resource in the Node API. Each advertised service has a 'type' property whose value is a Uniform Resource Name (URN), as well as its 'href' property which provides a URL to reach the service. The Node Service Types parameter repository provides implementers with the means to discover and disclose service type names (URNs) that are in use.

Its guidance contains the following requirements:

- Each entry MUST define a unique service type name (which is a URN).
- Each entry MUST have a short description and proponent(s).
- Each entry SHOULD provide a link to a specification for the service type, as well as specifying the IS-04 versions for which the entry is applicable.
- In the case of substantial revision to the service specification, a new service type name MUST be defined. Using versioned names is therefore RECOMMENDED.
- Additions and updates to this parameter repository may be submitted via a GitHub Pull Request (PR).

However, modifications to a parameter repository may be more closely controlled than this. For example, in the case of the Formats parameter repository, values SHALL only be added by a revision to an AMWA NMOS specification.
