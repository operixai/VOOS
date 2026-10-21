VOOS SOURCE BOOTSTRAP

What this is
- One GitHub Actions workflow that imports the OpenClaw source tree directly into the VOOS repository root.
- It keeps the upstream MIT license and records the exact upstream commit.
- It integrates a first VOOS voice dock into the existing native chat's Talk callback. It does not create a second gateway or agent session.
- The Obsidian file documents the required integration but does NOT implement a complete Obsidian adapter yet.
- A build is attempted after source import; the source commit remains even if build verification fails.

Install once
1. Open https://github.com/operixai/VOOS
2. Choose Add file -> Create new file.
3. Set the filename to: .github/workflows/bootstrap-voos.yml
4. Copy the content from the included .github/workflows/bootstrap-voos.yml file into GitHub's editor.
5. Commit the new file to main.
6. Open Actions -> "Bootstrap VOOS from OpenClaw source" -> Run workflow -> Run workflow.
7. Watch the workflow run. It commits the imported source to main before attempting install/build.

Do not add API keys, access tokens, or private Obsidian vault data to this repository.
