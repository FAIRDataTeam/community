# FAIR Data Point requirements and features

## FDP specification

From the [FDP specification v1.2]:

>The main goal of the FDP is to establish a common method for metadata provisioning and accessing and, as a consequence, provide to client applications a predictable way of accessing and interacting with metadata content.
>To fulfill this goal, this document contains a set of specifications *to help developers to extend the functionality of their applications* so these applications can also *behave as a FAIR Data Point*.

## FDP implementations

There are many ways to implement the [FDP specification v1.2], for example:

- **Act like an FDP**:
  Extend the functionality of an existing application so it behaves as an FDP.
- **Set up a document-based FDP**:
  As a minimal implementation, you can set up a static-file server that serves simple text documents containing the required RDF metadata.
- **Use the FDP reference implementation**:
  The [FDP reference implementation] was built by the creators of the FDP specification as an example of a fully featured application that conforms to the FDP specification.
  This implementation contains many convenient features that are *not* required by the specification.

>[!IMPORTANT]
>The [FDP specification v1.2] defines the required behavior of the *server* side.
>It does *not* define any requirements for *client* applications.
>For this reason, the [FDP client] and [FDP UI] are not considered part of the [FDP reference implementation].

An overview of FDP requirements and optional features can be found in the table below.

## Overview of features and requirements

>[!NOTE]
>This table is *not* normative.
>Refer to the FDP specification for normative requirements.

| feature description  | [FDP specification v1.2] requirement | document-based FDP | FDP reference implementation |
|---|---|---|---|
| root url resolves to DCAT (meta)data service description | ✓ | ✓ | ✓ |
| metadata exposed as RDF turtle/json-ld | ✓ | ✓ | ✓ |
| metadata links to profile with SHACL shapes | ✓ | ✓ | ✓ |
| SHACL shapes target `dcat:Resource` | ✓ | ✓ | ✓ |
| LDP containment statements | ✓ | ✓ | ✓ |
| metadata access control | ?<sup>*</sup> | ?<sup>**</sup> | ✓ |
| HTTP GET metadata | ✓ | ✓ | ✓ |
| HTTP POST metadata |   |   | ✓ |
| HTTP PUT metadata |   |   | ✓ |
| HTTP PATCH metadata |   |   |   |
| HTTP DELETE metadata |   |   | ✓ |
| OpenAPI/Swagger-UI API docs |   |   | ✓ |
| metadata validation |   |   | ✓ |
| user management |   |   | ✓ | 
| settings management |   |   | ✓ |
| basic search |   |   | ✓ |
| SPARQL query |   |   | ✓ |
| triple store backend |   |   | ✓ |
| modular resource definitions |   |   | ✓ |
| FDP-index functionality |   |   | ✓ |
| factory reset option |   |   | ✓ |
| label service |   |   | ✓ |
| autocomplete service |   |   | ✓ |

<sub>*: "Access control" is mentioned in [FDP specification v1.2] as part of the FDP infrastructure, but it is not an explicit conformance requirement.</sub>

<sub>**: Most static-file server applications support at least a rudimentary form of access control.


[FDP specification v1.2]: https://specs.fairdatapoint.org/v1.2/fdp-specs-v1.2.html
[FDP reference implementation]: https://github.com/FAIRDataTeam/FAIRDataPoint
[FDP client]: https://github.com/FAIRDataTeam/FAIRDataPoint-client
[FDP UI]: https://github.com/FAIRDataTeam/FAIRDataPoint-UI
