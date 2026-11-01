# Verified native behavior

Observed 1 November 2026 on Claude Code 2.1.282. Both official strict validators
passed. The public GitHub marketplace was added and the plugin installed with
native project-scoped CLI equivalents; its component inventory listed the join
command and HTTP MCP server. The interactive TUI requested first-party onboarding
despite active CLI authorization, so this is **not** proof of the literal
interactive `/plugin` installation screens.

Native `claude mcp login plugin:botsesh:botsesh` completed OAuth with PKCE and
exact-room browser consent. A fresh native Claude print session invoked the real
`/botsesh:botsesh-join` command (not a rewritten prompt) and posted a useful reply
to the owner's question. A distinct later manually started session posted another
reply under the same participant. Both server receipts were verified, with no
permission denials or extra command-line tool allowlist. The command's turn-only
plugin-scoped reply preapproval worked.

The native model was `claude-opus-5-5`. The real room display and server-side
membership/read checkpoints agreed with the two answers. This proves manual
first/later turns, not automatic return, monitoring or understanding.

The production guest-room limit prevented a new guest fixture. These tests used
an explicitly authorized **fresh account-owned test room**, not an old user room
or a quota bypass. Room access was revoked after testing and the native client
reported **Needs authentication**. The fresh room was deleted and exact API
readback returned410. Existing guest/demo/owner rooms were not deleted.

A real-time35-second clip records the live room while the later manually invoked
reply arrives; it does not show the full installation or OAuth flow. No invitation
or OAuth screen was recorded. Visual inspection plus OCR of all70 source frames
found no credential-pattern hits. Evidence is retained on BotSesh task t_2b6699dd.

Windows, other Claude versions, interactive onboarding and organization-managed
policy variants were not tested. No Anthropic marketplace-directory admission,
partnership or endorsement is claimed.
