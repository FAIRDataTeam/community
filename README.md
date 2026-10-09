# Welcome to the FAIR Data Point community

This repository provides an overview of the FAIR Data Point (FDP) ecosystem.
It also provides a place for high-level [discussions] and documents.

## FDP ecosystem

For an overview of all repositories, visit the [FAIRDataTeam] organization page.

Here's a summary of the core repositories:

- [fdp-specs/fdp-specs.github.io] (fdp-spec):
  The source of the [FDP specification].
- [FAIRDataTeam/FAIRDataPoint] (fdp):
  The server-based *reference implementation* of the [FDP specification].
  This is the core FDP application, providing a web API for metadata management, including Swagger-UI documentation, and optional index functionality.
- [FAIRDataTeam/FAIRDataPoint-UI] (fdp-ui):
  A browser-based user interface for the FDP *reference implementation*. (*under construction*)
- [FAIRDataTeam/FAIRDataPoint-client] (fdp-client):
  A browser-based user interface for the FDP. (*legacy*)

Tools:

- [LUMC-DCC/meta2fdp]:
  A Python framework for extracting and transforming metadata, and publishing it to an FDP instance
- [FAIRDataTeam/compose]:
  Docker Compose configuration examples for local test FDP deployments

[discussions]: https://github.com/FAIRDataTeam/community/discussions
[FAIRDataTeam]: https://github.com/FAIRDataTeam
[FAIRDataTeam/compose]: https://github.com/FAIRDataTeam/compose
[FAIRDataTeam/FAIRDataPoint]: https://github.com/FAIRDataTeam/FAIRDataPoint
[FAIRDataTeam/FAIRDataPoint-client]: https://github.com/FAIRDataTeam/FAIRDataPoint-client
[FAIRDataTeam/FAIRDataPoint-UI]: https://github.com/FAIRDataTeam/FAIRDataPoint-UI
[fdp-specs/fdp-specs.github.io]: https://github.com/fdp-specs/fdp-specs.github.io
[FDP specification]: https://fdp-specs.github.io
[LUMC-DCC/meta2fdp]: https://github.com/LUMC-DCC/meta2fdp
