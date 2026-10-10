# MLBN Tools Releases

Public distribution point for MLBN administrative utilities.

Release assets contain:

- the one-file `Install-MLBNTools.cmd` bootstrapper;
- an authenticated, encrypted manager package;
- an authenticated, encrypted catalog; and
- authenticated, encrypted utility packages.

The source code, tests, and build tooling are maintained separately in a private repository. A distribution password is required to decrypt the manager, catalog, and utility packages. The password is never embedded in this repository or its release assets.

## Installation

Download `Install-MLBNTools.cmd` and its matching `.sha256` file from the latest release. Verify the SHA-256 digest, then double-click the installer and enter the distribution password when prompted.

Unsigned PowerShell is launched with a process-scoped execution-policy bypass. The installer does not change the machine or user execution policy.

## Trust boundary

The packages are not Authenticode-signed. Confidentiality and integrity depend on custody of the shared distribution password, authenticated encryption, GitHub release transport, and published SHA-256 digests. Do not redistribute decrypted scripts or the password.

## License

No license is granted for redistribution, modification, or public reuse. All rights reserved.
