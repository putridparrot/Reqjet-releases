# Reqjet

An API client for Windows, macOS and Linux. Requests are saved as plain `.http` files, the same format
Visual Studio, VS Code REST Client and JetBrains IDEs use, so they live in your repository next to your code and
work in all of those tools.

- Send requests from a form or as `.http` text, with environments, OAuth 2.0, client certificates and proxies.
- Turn responses into tests (assertions, snapshots, OpenAPI contract checks) that also run in CI from the command line.
- JetBrains-style scripts, data-driven runs, runbooks, a mock server, a quick load test, and imports from
  curl, OpenAPI, Postman and browser recordings (HAR).

**[Website](https://www.reqjet.com)** · **[User guide](https://www.reqjet.com/docs)** ·
**[Samples to try](https://www.reqjet.com/docs/getting-started/samples/)**

## Download

Get the latest version from **[Releases](../../releases/latest)**:

| System | Install | Portable (no install) |
| --- | --- | --- |
| Windows (Store) | [Microsoft Store](https://apps.microsoft.com/detail/9PFCWG7138MW), or `winget install 9PFCWG7138MW -s msstore` | |
| Windows | `Reqjet-<version>-win-x64-setup.exe` (or `win-arm64`) | `Reqjet-<version>-win-x64.zip` |
| macOS | `Reqjet-<version>-osx-arm64.dmg` (Apple Silicon) or `osx-x64.dmg` (Intel) | `.zip` with `Reqjet.app` |
| Linux | `Reqjet-<version>-x86_64.AppImage` (most distributions) or `reqjet_<version>_amd64.deb` (Debian/Ubuntu: it adds [apt.reqjet.com](https://apt.reqjet.com), so `apt upgrade` updates it) | `.tar.gz` |
| Command line | `dotnet tool install -g Reqjet.Cli` ([NuGet.org](https://www.nuget.org/packages/Reqjet.Cli)). Offline: `Reqjet.Cli.<version>.nupkg` with `--add-source <its folder>` | |
| Samples | | `Reqjet-samples.zip`: ready-made requests against free public APIs |

The desktop downloads are self-contained: nothing else needs installing. They aren't code signed yet, so Windows
SmartScreen and macOS Gatekeeper ask before the first run (on Windows choose *More info* > *Run anyway*, or for a
`.zip` tick *Unblock* in its *Properties* before unzipping; on macOS choose *Open Anyway* under *System Settings* >
*Privacy & Security*). On Windows, the Microsoft Store version is signed by Microsoft, so it skips these checks, runs
with Smart App Control on, and updates itself. Each release lists SHA-256 checksums in `SHA256SUMS.txt`.

For managed Windows machines: `Reqjet-<version>-win-x64-setup.exe /VERYSILENT /ALLUSERS` installs for everyone.

## Feedback

Found a bug or want a feature? Open an [issue](../../issues).
