# 安装与使用

1. 从 GitHub Release 下载 `FlowFTP-0.4.0-macOS-arm64.pkg` 与 `SHA256SUMS`，在两份文件所在目录运行 `shasum -a 256 -c SHA256SUMS`，确认校验通过。
2. 双击安装包，按安装器提示，将 FlowFTP 安装至「应用程序」。应用包包含传输依赖，无需安装 Homebrew。
3. 打开「FlowFTP → 设置 → 通用」完成免费激活，选择简体中文、English 或跟随系统。回到工作台选择协议，输入主机、端口、用户名和密码。SFTP 需选择已核验的 `known_hosts` 文件。FTPS 可在「连接选项」中指定私有 CA。[激活说明](ACTIVATION.md)
4. 点击「连接」，右侧自动显示远程文件。常用站点可用「连接清单 → 保存当前连接」保存，下次直接选择。勾选记住密码时，凭据存入 macOS 钥匙串。使用 ⌘ 多选文件，再点击「上传」或「下载」。
5. 清单显示每个文件的状态、字节数和速度。同名时可保留并跳过、换名、覆盖当前项或覆盖本批全部同名项。下载完整后才替换已确认的本地文件。

代理默认留空直连。可在「连接选项」中填写 `socks5h://主机:端口` 或 `http://主机:端口`，该连接的读取和传输会使用指定代理。FTP 使用明文。若服务端支持，请选 FTPS 或 SFTP。

本预览构建的 PKG 未使用 Developer ID 签名，应用仅作本地签名，全包未公证。macOS 可能拦截从网络取得的安装包或应用。先核对来源和 SHA-256。如决定放行，仅针对该文件使用系统的「仍要打开」选项。企业设备也可能禁止放行。 [Apple 官方说明](https://support.apple.com/zh-cn/102445)

CLI 位于 `/Applications/FlowFTP.app/Contents/MacOS/flowftp`。运行 `help` 查看用法，运行 `capabilities` 核对实际协议支持。

卸载时退出程序，将「应用程序」里的 FlowFTP 移到废纸篓。
