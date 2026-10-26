# Matrix of Co-Creator（众创矩阵）

Windows Minecraft 启动器，提供游戏实例与整合包管理、下载更新以及账号管理界面。

**[下载 alpha.36 · Windows x64 安装包](https://github.com/SeasideH1/Matrix-of-Co-Creator/releases/download/v0.1.0-alpha.36/Matrix-of-Co-Creator-0.1.0-alpha.36-x64-Setup.exe)**

本仓库提供产品说明与安装包。安装包名称：`Matrix-of-Co-Creator-0.1.0-alpha.36-x64-Setup.exe`。

[中文隐私政策](#privacy-zh-cn) · [中文使用条款](#terms-zh-cn) · [中文许可说明](#license-zh-cn) · [English](#project-en-us)

## Status

**alpha.36 为审核预览，尚未完成真实 Minecraft 登录验收。** 此状态不代表 Microsoft 或 Mojang 批准。游戏实际启动仍要求在线验证 Microsoft 账号的 Java 版资格和玩家资料；验证失败会阻止启动。

**alpha.36 is a review preview; real Minecraft sign-in acceptance is not complete.** This status does not imply approval by Microsoft or Mojang. Actual game launches require online verification of a Microsoft account's Java Edition entitlement and profile. Failed verification blocks launch.

## Project zh-CN

- 需要 Windows x64、网络连接及合法取得的游戏和内容使用权。实际启动需要具备 Minecraft Java 版资格的 Microsoft 账号；所选游戏版本还需要兼容的 Java 运行时。
- 安装前保留重要数据备份。旧版迁移会保留旧安装及数据副本；回退使用旧副本，新版数据不会自动合并回去。保留副本中的个人数据需要另行处理。
- 本版更新项目展示信息、移除个人邮箱，并统一中英文隐私、条款和项目主页入口。
- 公开产品说明和版本更新以本 README 与 Releases 为准。本项目未在这里提供专用联系或反馈服务。

非 Minecraft 官方产品，未经 Mojang 或 Microsoft 批准，且与二者无关联。

## Privacy zh-CN

版本：0.1.0-alpha.36；更新日期：2026-10-24。以下适用于本客户端及配套平台服务。

**数据与接收方。** Microsoft 登录在系统浏览器的微软页面完成，客户端不收取微软密码。Microsoft、Xbox 和 Minecraft 服务处理授权、游戏资格和玩家资料校验。本机保存账号类型、玩家名、UUID、设置、实例路径、下载、任务和进程时长；凭据存入本机加密库，Windows 库密钥由当前用户的 DPAPI 保护。

平台登录向主服务提交短期 Minecraft access token 作官方核验，将 Minecraft UUID 与平台账号 ID 关联；不发送 Microsoft 刷新令牌，也不把原始 Minecraft token 写入账号数据库。平台保存资料、好友关系、申请、预设消息、邀请、评价、读取状态、资格及统计。玩家可见公开资料和参与的互动，公开资料不包含 Minecraft UUID。可信游戏服务端提供 UUID、入服/离服事件以计算服务端时长，与本机进程时长分开。平台服务器和备份位于中国；其他远程可能有不同运营者和政策，请核对地址与发布者指纹。

内容远程收到限定范围的签名资格、内容请求及连接信息，用于授权和传输。下载优先复用已校验缓存；Minecraft 和受支持加载器优先官方源，失败或持续低速时使用 BMCLAPI；Java 优先 TUNA，后备 Adoptium，元数据与摘要来自官方。整合包也可能使用签名清单中的第三方地址。下载站点及 GitHub 接收普通网络连接信息；不会向其他源复制认证头。文件校验不代表内容再分发许可。

**诊断与保存期限。** 诊断可能包含错误类别、版本、阶段、进度及脱敏消息；仅在预览报告和接收地址并明确确认后发送，不按平台账号建立索引。发送前请检查，自由文本脱敏不能保证绝对完整。本机最多保存 20 组诊断，启动时清理超过 30 天的报告；接收服务详细样本和回执最多保存 30 天，聚合最多 180 天。平台注销无法按账号定位这些报告。

活跃平台数据保存至账号注销；短期挑战与凭据按有效期清理。注销申请立即停用账号、撤销会话，进入 30 天冷静期；好友和搜索只显示注销状态、平台 ID、创建日期与申请日期。期满删除账号、UUID 关联、社交消息、资格、统计及关联记录。必要安全审计最多 180 天，并移除直接关联的旧记录、仅保留最小伪名记录；备份最多 30 天。外置删除记录只保留带密钥的账号伪名和生命周期日期至恢复窗口结束，恢复服务前必须重放删除记录并完成清理。

**你的操作。** 在“设置 → 账号与启动”移除本机账号，登录平台后可导出 JSON 或申请注销。导出包含本人平台与本机账号/实例元数据，不含密码、访问/刷新/恢复令牌或他人私密资料。冷静期内须重新进行 Microsoft 验证并明确点击“撤销账号注销”；重新登录不会自动恢复，期满删除不可恢复。可在个人资料界面更正支持的字段，在 [Microsoft 应用授权管理](https://account.live.com/consent/Manage)撤销授权。

平台注销不删除 Microsoft 账号、购买、游戏文件或存档。移除本机账号清除该账号凭据和实例绑定；本机设置、日志、存档、迁移副本及导出文件由你自行保管和清理。不要公开密码、令牌或账号导出文件。重要变更将在本页及发布说明披露。

## Terms zh-CN

版本：0.1.0-alpha.36；更新日期：2026-10-24。

实际启动 Minecraft，包括源码和开发运行，均要求在线验证 Microsoft 账号的 Java 版资格与玩家资料；服务拒绝、网络不可用或资格缺失时阻止启动。离线身份、第三方身份、缓存资格和 OPL 联网不能代替官方资格与服务器准入。受控测试替身不启动 Minecraft，也不构成开发启动例外。

你须自行取得游戏、模组、资源及服务器内容的使用权，遵守适用条款和各组件许可。启动器不出售或授予 Minecraft 购买资格。不得冒用身份、绕过权限或分发无权分发的内容；添加远程前应核对地址及签名发布者。

本版仍为 alpha。签名更新与摘要校验不保证没有缺陷或第三方内容具有许可。安装、升级或删除重要数据前请保留备份。在线服务可能因维护、故障、资格或第三方限制而不可用，不承诺永久在线。账号数据与注销规则见[隐私政策](#privacy-zh-cn)。

本条款不缩减 AGPL 授予的软件权利，冲突时以许可证为准。适用法律允许范围内，软件按 AGPL 第 15–17 节提供无担保及责任限制，不排除法律不允许排除的权利。

在适用法律允许的最大范围内，运营者代表 Microsoft 排除与本应用有关的所有保证及责任；本条保留适用法律规定不得排除的权利。依据：[Microsoft identity platform 使用条款第 2.1.6 节](https://learn.microsoft.com/en-us/legal/microsoft-identity-platform/terms-of-use)。

## License zh-CN

项目有权授权的自有启动器代码采用 **GNU Affero General Public License v3.0 only（AGPL-3.0-only）**。允许依许可证使用、研究、修改和再分发，包括商业使用；分发以及修改后网络服务的对应源码义务依许可证执行。此下载仓库不声称提供完整源码；这不改变许可证规定的义务。

完整许可证、项目声明和第三方声明随安装包提供。第三方代码、既有贡献、字体、图像、商标、Minecraft、模组及整合包保留各自权利，不因本项目许可被重新授权。软件许可不授予额外商标权。项目主页即本 README。

## Project en-US

Matrix of Co-Creator is a Windows Minecraft launcher with game instance and modpack management, downloads, updates and account controls.

**[Download alpha.36 for Windows x64](https://github.com/SeasideH1/Matrix-of-Co-Creator/releases/download/v0.1.0-alpha.36/Matrix-of-Co-Creator-0.1.0-alpha.36-x64-Setup.exe)**

- Requires Windows x64, a network connection and the rights to use the game and selected content. Actual launches require a Microsoft account with Minecraft Java Edition entitlement and a compatible Java runtime for the chosen game version.
- Back up important data before installation. Migration retains the old installation and data snapshot. Rollback uses that snapshot; newer data is not merged back automatically. Handle personal data in retained copies separately.
- This version removes personal email information and consolidates privacy, terms and project links in both languages.
- This repository provides product information and installers. This README and Releases carry public updates; no dedicated contact or feedback service is offered here.

Not an official Minecraft product. Not approved by or associated with Mojang or Microsoft.

## Privacy en-US

Version 0.1.0-alpha.36; updated 2026-10-24. This policy applies to this client and its matching platform service.

**Data and recipients.** Microsoft sign-in occurs on Microsoft's page in a system browser; the client does not collect Microsoft passwords. Microsoft, Xbox and Minecraft services handle authorization, entitlement and profile verification. Local data includes account type, name, UUID, settings, instance paths, downloads, tasks and process duration. Credentials are encrypted locally; Windows protects the vault key with the current user's DPAPI.

Platform sign-in sends a short-lived Minecraft access token to the platform for independent official verification and associates the UUID with a platform account ID. Microsoft refresh tokens are not sent, and raw Minecraft tokens are not persisted in the account database. The platform stores profiles, friendships, requests, preset messages, invitations, ratings, read state, eligibility and statistics. Players see public profiles and their interactions; public profiles exclude Minecraft UUID. Trusted game servers report UUID and join/leave events for server playtime, separate from local process duration. Platform servers and backups are in China. Other selected remotes may have different operators and policies; check their addresses and publisher fingerprints.

Content remotes receive scoped signed eligibility, content requests and connection information for authorization and transfer. Downloads reuse verified cache where possible. Minecraft and supported loaders prefer official hosts, with BMCLAPI fallback for failures or sustained low speed. Java prefers TUNA with Adoptium fallback and official metadata/digests. Modpacks may use third-party URLs in signed manifests. Download sites and GitHub receive ordinary network information; credentials are not copied to other origins. Hash verification does not establish redistribution permission.

**Diagnostics and retention.** Reports may contain error categories, versions, phases, progress and redacted messages. They are sent only after you preview the report and destination and explicitly confirm. They are not indexed by platform account. Review free text before sending; redaction is not an absolute guarantee. The client keeps at most 20 report groups and removes reports older than 30 days at startup. The collector keeps detailed samples and receipts for at most 30 days, aggregates for at most 180 days. Account deletion cannot identify these reports by account.

Active platform data remains until account deletion; short-lived challenges and credentials expire. Deletion immediately disables the account and revokes sessions, followed by a 30-day cooling period. Friends and search show only deletion status, platform ID, creation and request dates. Final purge erases the account, UUID link, social records, messages, eligibility, statistics and related records. Minimal security audits last at most 180 days, with directly linked older records removed and only minimal pseudonymous records retained. Backups last at most 30 days. An external deletion journal stores keyed account pseudonyms and lifecycle dates through the recovery window; restored services must replay it and complete cleanup before serving.

**Your controls.** Settings → Accounts & launch supports local account removal and, when signed in, JSON export and platform deletion. Exports contain your platform and local account/instance metadata, excluding passwords, access/refresh/recovery tokens and other players' private profiles. During the cooling period, recovery requires fresh Microsoft verification and an explicit Cancel account deletion action. Signing in alone does not restore the account; final purge is irreversible. Edit supported fields in your profile and revoke consent in [Microsoft app permissions](https://account.live.com/consent/Manage).

Platform deletion does not delete Microsoft accounts, purchases, games or saves. Removing a local account clears its credentials and instance bindings. You control local settings, logs, saves, migration snapshots and exports. Do not publish passwords, tokens or account exports. Material changes will appear here and in release notes.

## Terms en-US

Version 0.1.0-alpha.36; updated 2026-10-24.

Every actual Minecraft launch, including source and development runs, requires online Microsoft Java Edition entitlement and profile verification. Service denial, network failure or missing entitlement blocks launch. Offline or third-party identities, cached proofs and OPL connectivity do not substitute for official entitlement or server admission. Controlled test doubles do not launch Minecraft and provide no development launch exception.

Obtain the rights required for games, mods, resources and server content, and comply with applicable terms and component licenses. The launcher does not sell or grant Minecraft ownership. Do not impersonate others, bypass access controls or redistribute content without permission. Check remote addresses and signing publishers before adding a remote.

This is alpha software. Signed updates and digest checks do not guarantee absence of defects or permission for third-party content. Back up important data before installation, upgrades or deletion. Services may be unavailable because of maintenance, faults, eligibility or third-party restrictions; permanent availability is not promised. Account rules are in the [privacy policy](#privacy-en-us).

These terms do not reduce rights granted by AGPL; the license prevails in a conflict. AGPL sections 15–17 govern warranty and liability to the extent permitted by law, without excluding rights that cannot lawfully be excluded.

To the fullest extent permitted by applicable law, the operator disclaims all warranties and liability on behalf of Microsoft in connection with this application; rights that cannot lawfully be excluded remain unaffected. Basis: [Microsoft identity platform terms of use, section 2.1.6](https://learn.microsoft.com/en-us/legal/microsoft-identity-platform/terms-of-use).

## License en-US

Project-owned launcher code that the owner has the right to license uses **GNU AGPL-3.0-only**. Use, study, modification, redistribution and commercial use are permitted subject to that license, including corresponding-source obligations for distribution and modified network services. This download repository does not claim to provide the complete source; license obligations remain unchanged.

The complete license, project notice and third-party notices are included in the package. Third-party code, pre-existing contributions, fonts, images, trademarks, Minecraft, mods and modpacks retain their respective rights and are not relicensed by this project. No additional trademark rights are granted. This README is the project home.
