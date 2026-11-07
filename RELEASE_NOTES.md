# KryptoCore MSG 0.1.0-alpha.2-preview.4

Development preview following 0.1.0-alpha.1. Existing identity, invitation and
encryption formats are unchanged.

- Chat-focused interface with a compact borderless window, navigation rail, searchable contacts and message bubbles.
- Address requests with accept/reject/block; approval opens the chat on both sides.
- Save contacts from a chat, preserve the active connection when reselecting it, and check saved keys on reconnect.
- Bounded per-contact session messages/drafts; clear them on lock, close or identity change.
- Prompt for a file location when no receive folder is selected; preserve existing files.
- Show a green channel marker only after both encrypted ready confirmations.
- Reject missing/corrupt ready confirmations and modified chat ciphertext in protocol tests.

Tor and the self-contained Windows runtime are bundled. The executable is
unsigned. No independent audit is claimed. Local regression uses an isolated
loopback SOCKS bridge with real cryptographic workers; a full public-Tor and
two-computer check remain pending for this exact preview. There is no voice,
offline delivery or persistent history. Files are limited to 16 MiB.

SHA256SUMS.txt and RELEASE_MANIFEST.json identify the archive, executable,
private source commit and validation scope. Retain backups and use test data.
