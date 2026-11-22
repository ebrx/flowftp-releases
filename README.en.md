# FlowFTP

[简体中文](README.md) · English

FlowFTP is a dual-pane Mac app for FTP, explicit and implicit FTPS, and SFTP. Connect to open the remote directory immediately. Select multiple files to upload or download and follow each transfer in the queue. On a conflict, keep the existing file, rename the incoming file, replace one, or replace all conflicts in the current batch. The interface supports English, Simplified Chinese, and the system language.

Download the arm64 PKG and its checksum from [GitHub Releases](https://github.com/ebrx/flowftp-releases/releases). This preview requires Apple Silicon and macOS 27.0 or later. Verify the download with `shasum -a 256 -c SHA256SUMS`, then open the package and follow Installer. The preview package is unsigned and has not been notarized.

Open FlowFTP from Applications. In **FlowFTP → Settings → General**, choose your language and complete free offline activation before transferring files. [Activation instructions](ACTIVATION.en.md)

Save frequently used sites from the connection list. Choose a saved connection and click **Connect** to reopen its remote directory. If you choose to remember connection credentials, FlowFTP stores them in macOS Keychain.

The operation video shows how to save and reuse a connection, upload a batch, handle a name conflict, and follow transfer progress. The recording uses synthetic files and an offline demo server view.
