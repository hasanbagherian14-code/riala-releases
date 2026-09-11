# RIALA Releases

Official public release channel for RIALA desktop updates.

This repository contains only public release binaries, release notes, and the updater manifest. No private source code, databases, backups, credentials, or user data are published here.

## Current stable release

RIALA v3.4.4 is the current published stable release. See the Releases section of this repository.

## Important Portable v3.3.2 migration notice

Portable v3.3.2 contains an updater handoff defect in the already-running application. Portable v3.3.2 must not attempt an automatic self-update to v3.4.4.

Portable v3.3.2 users should perform one manual transition:

1. Close RIALA completely.
2. Keep the existing Portable executable as a temporary rollback copy.
3. Download RIALA_Portable_v3.4.4.exe from the v3.4.4 release.
4. Place and run v3.4.4 from the intended Portable location.
5. Verify normal startup and a healthy database status.
6. Remove the old Portable copy only after verification.

Once running v3.4.4, future Portable updates can use the corrected updater path.

The public release-manifest.json remains intentionally pinned to v3.3.2 at this stage to protect existing Portable v3.3.2 users from the known handoff defect.
