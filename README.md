# Matrix of Co-Creator（众创矩阵）

**非 Minecraft 官方产品，未经 Mojang 或 Microsoft 批准，且与二者无关联。**

开发与运营：**SeasideH1**，联系：[qq1602770686@outlook.com](mailto:qq1602770686@outlook.com)。Windows Minecraft Java 版启动器，提供实例与整合包管理、下载更新及账号操作。

[下载](#download) · [中文隐私政策](#privacy-zh-cn) · [中文使用条款](#terms-zh-cn) · [许可](#license-zh-cn) · [English](#project-en-us)

## Download

**[下载 alpha.37 · Windows x64 安装包](https://github.com/SeasideH1/Matrix-of-Co-Creator/releases/download/v0.1.0-alpha.37/Matrix-of-Co-Creator-0.1.0-alpha.37-x64-Setup.exe)** · [版本说明](https://github.com/SeasideH1/Matrix-of-Co-Creator/releases/tag/v0.1.0-alpha.37)

安装包：`Matrix-of-Co-Creator-0.1.0-alpha.37-x64-Setup.exe`，181,672,094 字节。

SHA-256：`b44dc51d078e077afec8529efacc7a8eddd8d71ccdc4351056a347640ef55ae6`

## Status

**alpha.37 为审核预览，真实 Minecraft 登录尚未通过验收。** 每次实际启动须在线核验 Microsoft 账号的 Minecraft Java 版资格与玩家资料；验证失败或不可用时阻止启动。

**Alpha.37 is a review preview; live Minecraft sign-in acceptance is incomplete.** Every actual launch verifies Microsoft Java Edition entitlement and the player profile online. Failed or unavailable verification blocks launch.

## Project zh-CN

需要 Windows x64、网络连接、合法取得的游戏与内容使用权，以及所选游戏版本兼容的 Java。Minecraft 本体、元数据、库文件与资源仅使用官方源；第三方加载器使用独立来源策略。Java 保持 TUNA 优先、Adoptium 后备。

本版补充直接联系与完整非官方声明，调整 Minecraft 下载来源，并随安装器提供对应源码及构建说明。安装升级前请备份重要数据；旧版迁移保留的安装和数据副本可用于回退，新版数据不会自动合并回旧版。产品、隐私和源码问题可直接联系 [SeasideH1](mailto:qq1602770686@outlook.com)。

## Privacy zh-CN

版本：0.1.0-alpha.37；更新日期：2026-10-26。本文适用于本客户端及配套主服务；部署者应同步启用所述数据清理与恢复流程。

### 项目与数据接收方

项目为 **Matrix of Co-Creator（众创矩阵）**，开发与运营者为 **SeasideH1**，联系：[qq1602770686@outlook.com](mailto:qq1602770686@outlook.com)。公开说明见[项目主页](https://github.com/SeasideH1/Matrix-of-Co-Creator/#project-zh-cn)。平台服务器和备份位于中国。

平台与整合包远程服务按客户端发行配置连接。如选择其他远程，其运营者、内容与政策可能不同；请先核对客户端显示的地址和发布者指纹。GitHub 项目主页访问由 GitHub 处理网络请求。

### 数据流与用途

| 类别 | 处理位置、接收者与用途 |
|---|---|
| Microsoft / Xbox / Minecraft 登录 | 系统浏览器打开微软授权页；客户端不收取微软密码。客户端与 `login.microsoftonline.com`、Xbox Live / XSTS 及 `api.minecraftservices.com` 完成授权、Java 资格和玩家资料校验。Microsoft 自行处理其登录数据。 |
| 本机游戏账号 | 账号类型、玩家名、Minecraft UUID、设置、实例路径、下载记录、任务与本机进程时长保存在本机。Microsoft 刷新凭据和短期 Minecraft 凭据存入本机加密凭据库；Windows 使用当前用户的 DPAPI 保护库密钥。 |
| 平台身份 | 在你登录平台时，客户端向主服务提交短期 Minecraft access token，由主服务向官方核验，建立平台 ID 与 Minecraft UUID 的对应关系；Microsoft 刷新令牌不发给主服务。该验证流程不把原始 Minecraft token 写入账号数据库。平台会话凭据留在本机加密库，服务端保存用于验证/撤销的摘要和期限。 |
| 资料与社交 | 主服务保存昵称、平台 ID/标签、所选地区/简介、好友关系与申请、预设消息、邀请、评价和读取状态，用于展示与互动。其他玩家可见公开资料和其参与的互动；Minecraft UUID 不作为公开个人资料返回。 |
| 游戏与下载 | 可信游戏服务端上报 Minecraft UUID、入服/离服及相关事件以计算平台时长、状态和资格；本机进程时长与服务端入服时长分开。远程服务收到限定范围的签名资格、内容请求及连接网络地址，用于私有内容授权、限流和传输。OPL 提供联网，不能代替游戏资格验证。 |
| 诊断 | 客户端整理错误类别、错误码、软件/系统/游戏/Java 版本、阶段、进度及经过脱敏的错误信息/栈。不会自动上传：先显示报告和接收地址，再由你明确确认发送。接收端不按平台账号关联报告；自由文本可能包含个人信息，请在发送前检查预览。 |

下载默认先复用通过摘要校验的本机缓存。Minecraft 本体、版本元数据、库文件和资源仅从官方地址下载；官方源失败时显示错误，不切换至镜像。第三方加载器按各自来源策略下载。Java 包优先清华 TUNA，后备为 Adoptium 官方发布地址，元数据及摘要来自官方。下载站点会接收普通连接信息；不会继承平台资格或其他源的认证头。整合包自身可使用签名清单中的第三方下载地址或远程压缩包，公开说明见[项目主页](https://github.com/SeasideH1/Matrix-of-Co-Creator/#project-zh-cn)。文件摘要用于验证完整性；内容的使用与分发按其许可执行。

### 保存期限

- 活跃平台账号：保存为提供账号、社交、资格及统计功能所需的数据，直至你申请并完成注销。短期挑战、会话、恢复凭据按各自到期时间失效并清理。
- 注销冷静期：申请后立即停用账号并撤销平台会话。30 天内保存恢复所需数据；好友和搜索只显示“已注销”、平台账号 ID、创建日期和申请注销日期，不能进行社交互动。
- 30 天到期：清理账号、UUID 绑定、社交/消息、邀请/评价、资格、统计、事件和关联缓存，包括上述展示记录。后续再次验证将建立新的平台账号。
- 必要安全审计：最多 180 天。删除清理去除可直接关联的旧记录，仅保留必要动作、时间及带密钥的账号伪名等最小记录；不用于恢复账号资料。
- 滚动数据库备份：最多 30 天。外置删除记录使用带密钥的账号伪名，不含玩家名或 Minecraft UUID，完成删除/撤销后保留至恢复窗口结束。恢复备份必须先重放删除记录，过期备份或缺失/不匹配的记录不得上线。
- 诊断：客户端最多保存 20 组，启动时清理超过 30 天的报告；接收服务详细样本和去重回执最多 30 天、聚合最多 180 天。这些报告没有平台账号索引，平台注销不能据账号 ID 定位删除。
- 本机数据由你控制：移除游戏账号清除该账号凭据和实例绑定；平台退出清除本机会话。实例、游戏存档、任务/日志与设置不随平台注销删除，保留至你自行清理。旧版迁移保留的副本和自行复制的导出文件也需要你另行处理。清理会在服务维护/下次启动时执行；服务离线时不会提供这些数据，恢复服务前先执行清理。

### 访问、更正、导出与注销

在“设置 → 账号与启动”可以选择游戏账号、移除本机游戏账号，登录平台后可点击“导出我的账号数据”保存 JSON。导出包括你的平台资料、本人参与的社交记录、统计和必要审计，以及本机账号/实例元数据，不包含访问/刷新/恢复令牌、密码或其他玩家的私密账号资料。它是数据副本，不是登录凭据备份或恢复账号工具；请妥善保存。

选择“注销平台账号”，阅读范围并确认后进入 30 天冷静期。期间重新验证微软账号只提供恢复选择，**不会自动撤销注销**；须再点击“撤销账号注销”。期满删除后不可恢复。平台注销不会注销微软账号或取消游戏购买，也不删除游戏文件/存档；你可在[微软应用授权管理](https://account.live.com/consent/Manage)中撤销应用授权。

资料更正可在个人资料界面操作。不要公开密码、令牌或账号导出文件。重要处理规则变更将更新[项目主页](https://github.com/SeasideH1/Matrix-of-Co-Creator/#project-zh-cn)和发布说明；客户端登录、账号及关于页面均提供隐私政策入口。

## Terms zh-CN

版本：0.1.0-alpha.37；更新日期：2026-10-26。

项目：**Matrix of Co-Creator（众创矩阵）**。开发与运营：**SeasideH1**，联系：[qq1602770686@outlook.com](mailto:qq1602770686@outlook.com)。

### 软件许可与服务

本项目有权授权的自有源代码采用 **GNU Affero General Public License v3.0 only（AGPL-3.0-only）**；完整条文随安装包提供，公开许可说明见[项目主页](https://github.com/SeasideH1/Matrix-of-Co-Creator/#license-zh-cn)。你可依照该许可证使用、研究、修改和再分发，包括商业使用。分发和修改后网络服务的对应源码义务按许可证执行。第三方组件、图标/素材与整合包依各自许可；本条款不将它们自动重新许可。软件名称和第三方商标不会因源码许可而获得额外商标授权。

这些服务说明不缩减 AGPL 已授予的软件权利；若与 AGPL 冲突，以 AGPL 为准。项目主页：[Matrix of Co-Creator](https://github.com/SeasideH1/Matrix-of-Co-Creator/#project-zh-cn)。安装包提供经过隐私清理的对应源码、构建说明及所需许可声明。服务自托管者需说明自己的运营主体和数据政策。

安装后在 `resources/source/Matrix-of-Co-Creator-0.1.0-alpha.37-source.zip` 取得本启动器的对应源码，在 `resources/source/README.build.md` 查看构建说明；不包含独立主服务或游戏适配器。

### 游戏身份与内容

每次实际启动 Minecraft 前，包括开发及源码运行，必须在线验证 Microsoft 账号的 Java 版资格及玩家资料。服务拒绝、网络不可用或资格缺失时阻止启动，不以独立离线身份、第三方身份或断网缓存代替。假身份仅用于不启动 Minecraft 的受控测试替身，不构成开发启动例外。OPL 不授予游戏资格或服务器准入。当前认证验收状态见[当前状态](https://github.com/SeasideH1/Matrix-of-Co-Creator/#status)。

你须自行获得 Minecraft、模组、资源、服务器及其他内容所需权利，并遵守适用的 Minecraft 条款与各组件许可。启动器不出售或授予 Minecraft 购买资格。文件摘要用于验证完整性；内容的使用与分发按其许可执行。添加远程前核对地址及签名发布者；不上传或分发你无权分发的内容，不冒用他人身份或绕过服务权限。

### 数据与账号

数据类别、接收者、期限及操作见[隐私政策](https://github.com/SeasideH1/Matrix-of-Co-Creator/#privacy-zh-cn)。平台无需另设密码，通过官方游戏身份验证建档。你可导出数据、移除本机凭据或申请平台注销；注销有 30 天冷静期，期满删除账号数据，必要审计最多 180 天、备份最多 30 天。冷静期内重新验证后须明确撤销，重新登录不会自动恢复。平台注销与微软账号删除、游戏文件删除是不同操作。

### 更新、恢复与责任

本版本仍为 alpha。签名与摘要分别用于验证发布来源和文件完整性；第三方内容适用各自许可。品牌迁移保留旧版安装及本机数据副本，回退后使用旧副本；新版本产生的数据不会自动反向合并。请在安装、升级或删除重要文件前保留可用备份。保留旧副本也意味着需要另行处理其中的个人数据。

软件按 AGPL 第 15–17 节在适用法律允许范围内提供无担保及责任限制，不排除法律不允许排除的权利。在线服务可能因维护、故障、资格或依赖服务限制而不可用；不承诺永久在线。重要行为或数据处理变更会在发布说明和政策中披露。公开更新见[项目主页](https://github.com/SeasideH1/Matrix-of-Co-Creator/#project-zh-cn)。

在适用法律允许的最大范围内，运营者代表 Microsoft 排除与本应用有关的所有保证及责任；本条保留适用法律规定不得排除的权利。依据：[Microsoft identity platform 使用条款第 2.1.6 节](https://learn.microsoft.com/en-us/legal/microsoft-identity-platform/terms-of-use)。

## License zh-CN

项目有权授权的自有启动器代码采用 **GNU AGPL-3.0-only**，允许依许可使用、研究、修改、再分发与商业使用。分发及修改后网络服务的对应源码义务按许可证执行。完整许可证、项目声明与第三方声明随安装包提供。

安装后的对应源码位于 `resources/source/Matrix-of-Co-Creator-0.1.0-alpha.37-source.zip`，构建说明位于 `resources/source/README.build.md`；此源码包对应启动器，不包含独立主服务或游戏适配器。源码包 SHA-256：`c000d149ce46b10a52b3e39eb134d1253bc1930e29acdd3acb0b24f79b2d476d`。

第三方代码、既有贡献、字体、图像、商标、Minecraft、模组与整合包保留各自权利；本项目许可不重新授权这些内容，也不授予额外商标权。

## Project en-US

**Not an official Minecraft product. Not approved by or associated with Mojang or Microsoft.**

Developer/operator: **SeasideH1**, [qq1602770686@outlook.com](mailto:qq1602770686@outlook.com). Matrix of Co-Creator is a Windows Minecraft Java Edition launcher for managing instances, modpacks, downloads, updates and accounts.

**[Download alpha.37 for Windows x64](https://github.com/SeasideH1/Matrix-of-Co-Creator/releases/download/v0.1.0-alpha.37/Matrix-of-Co-Creator-0.1.0-alpha.37-x64-Setup.exe)** · [Release notes](https://github.com/SeasideH1/Matrix-of-Co-Creator/releases/tag/v0.1.0-alpha.37)

Requires Windows x64, a network connection, rights to the game and selected content, and a compatible Java runtime. Minecraft game files, metadata, libraries and assets use official sources only. Third-party loaders have separate source policies. Java remains TUNA-first with Adoptium fallback.

This version adds direct contact and the complete unofficial-product notice, updates Minecraft download sources, and includes corresponding source and build instructions with the installer. Back up important data before installation or upgrade. Migration retains old installation/data snapshots for rollback; new data is not merged back automatically. Contact [SeasideH1](mailto:qq1602770686@outlook.com) for product, privacy or corresponding-source questions.

## Privacy en-US

Version 0.1.0-alpha.37; updated 2026-10-26. This policy applies to this client and its matching platform service. Operators must deploy the described deletion and recovery implementation.

### Project and recipients

The project is **Matrix of Co-Creator**. Developer/operator: **SeasideH1**, [qq1602770686@outlook.com](mailto:qq1602770686@outlook.com). Public information is available on the [project home](https://github.com/SeasideH1/Matrix-of-Co-Creator/#project-en-us). Platform servers and backups are in China.

The client connects to platform and content services using its distribution configuration. Other selected remotes can have different operators and policies. Check their addresses and publisher fingerprints. GitHub receives ordinary network requests when you open the project home.

### Data and purposes

Microsoft sign-in takes place in a browser on Microsoft's site; the client does not ask for your Microsoft password. It contacts Microsoft identity, Xbox Live / XSTS and `api.minecraftservices.com` to authorize and verify Java Edition entitlement and profile. Microsoft handles its own sign-in data.

Locally the client stores game account type/name/UUID, settings, instance paths, downloads, tasks and process duration. Microsoft refresh credentials and short-lived Minecraft credentials are encrypted locally; on Windows the vault key is protected by the current user's DPAPI. Platform sign-in sends a **short-lived Minecraft access token to the platform service** for independent official verification and associates the Minecraft UUID with a platform account ID. It does not send your Microsoft refresh token. This verification does not persist the raw Minecraft token in the account database. Local platform credentials use the encrypted vault; the service stores verification/revocation hashes and expiry data.

The platform stores profile fields, friendships and requests, preset messages, invitations, ratings and read state to provide social features. Players can see public profiles and interactions they participate in; Minecraft UUID is not included in public profiles. Trusted game servers report UUID, join/leave and related events for eligibility, status and server playtime. Local process time is separate. A content remote receives scoped signed eligibility credentials, content requests and ordinary connection addresses for authorization and transfer limits. OPL provides connectivity, not game entitlement.

Downloads first reuse verified local cache where possible. Minecraft game files, version metadata, libraries and assets are downloaded only from official hosts. Official-source failures are reported without switching to a mirror. Third-party loaders use their own source policies. Java packages prefer TUNA with fallback to Adoptium's official release; official metadata supplies the expected digest. Download sites receive ordinary connection information, without credentials copied from other origins. Modpacks may use addresses in signed manifests or remote compressed bundles. See the [project home](https://github.com/SeasideH1/Matrix-of-Co-Creator/#project-en-us). File digests verify integrity; use and distribution of content are governed by its license.

Diagnostics contain selected error categories/codes, software/system/game/Java versions, phase/progress and redacted messages/stacks. **Reports upload only after you preview and confirm the destination and report.** They are not indexed by platform account. Free text may contain personal information; check the preview before sending.

### Retention

- Active platform profile, social, entitlement and statistics data remains until account deletion. Short-lived challenges, sessions and recovery credentials expire and are cleaned up.
- A deletion request immediately disables the account and revokes sessions. A 30-day cooling period retains recovery data. Friends/search show only deactivated status, platform ID, creation date and deletion-request date; interactions are disabled.
- At the end of 30 days the service erases the account, UUID association, social/messages, invitations/ratings, entitlements, statistics, events, linked caches and displayed deletion record. Later registration creates a new account.
- Minimal security audits are retained for at most 180 days. Directly linked older records are removed during purge; necessary lifecycle actions/timestamps and keyed account pseudonyms remain, without restorable profile data.
- Rolling database backups last at most 30 days. An external deletion journal stores keyed platform ID pseudonyms and lifecycle dates, not player names or Minecraft UUIDs, through the recovery window after purge/cancellation. A restored database must replay that journal before serving. Expired backups or missing/mismatched journals cannot go live.
- The client keeps at most 20 diagnostic groups and removes reports older than 30 days at startup. The collector keeps detailed samples and deduplication receipts for at most 30 days and aggregates for at most 180 days. Because they lack a platform account index, account deletion cannot identify a report.
- Local files remain under your control. Removing a game account deletes its local credentials and instance bindings; signing out clears local platform credentials. Platform deletion does not remove local games, saves, tasks/logs or settings. Retained migration snapshots and exported files require separate handling. Cleanup runs during service maintenance or before restarted service becomes available.

### Your controls

Use Settings → Accounts & launch to remove local game accounts and, while signed in, export your platform data as JSON. The export includes your profile, interactions you participate in, statistics, minimal audits and local account/instance metadata. It excludes passwords, access/refresh/recovery tokens and other players' private account profiles. Protect the exported file; it is not an account restoration or credential backup.

Choose Delete platform account and explicitly confirm. During 30 days, fresh Microsoft verification offers recovery but **does not cancel deletion automatically**; select Cancel account deletion explicitly. After final purge the account cannot be restored. This does not delete your Microsoft account, purchases, game files or saves. Manage Microsoft consent at [Microsoft app permissions](https://account.live.com/consent/Manage).

Edit supported fields in your profile. Do not publish passwords, tokens or exported account data. Material changes will be reflected on the [project home](https://github.com/SeasideH1/Matrix-of-Co-Creator/#project-en-us) and in release notes. The sign-in, account and About screens provide the privacy policy link.

## Terms en-US

Version 0.1.0-alpha.37; updated 2026-10-26.

Project: **Matrix of Co-Creator**. Developer/operator: **SeasideH1**, [qq1602770686@outlook.com](mailto:qq1602770686@outlook.com).

### Software and service

Project-owned source code that the owner has the right to license is offered under **GNU AGPL-3.0-only**. The complete license is included in the package; see the public [license notice](https://github.com/SeasideH1/Matrix-of-Co-Creator/#license-en-us). The license allows use, study, modification, redistribution and commercial use, subject to its requirements, including corresponding source obligations for distribution and modified network services. Third-party components, artwork and modpacks retain their own terms; they are not automatically relicensed. No additional trademark rights are granted by the source license.

These service terms do not reduce AGPL rights; AGPL prevails in case of conflict. Project home: [Matrix of Co-Creator](https://github.com/SeasideH1/Matrix-of-Co-Creator/#project-en-us). The package includes a privacy-cleaned corresponding source snapshot, build instructions and required notices. Independent operators must identify themselves and publish their own accurate data policies.

After installation, the launcher corresponding source is located at `resources/source/Matrix-of-Co-Creator-0.1.0-alpha.37-source.zip`, with build instructions at `resources/source/README.build.md`. It does not include the separate main service or game adapter.

### Identity and content

Every actual Minecraft launch, including source and development runs, verifies the Microsoft account's Java Edition entitlement and profile online. Service denial, network failure or lack of entitlement prevents launch; standalone offline identities, third-party identities and cached offline proofs cannot substitute. Synthetic identities are limited to controlled test doubles that do not launch Minecraft; they provide no development launch exception. OPL provides connectivity, not entitlement or server admission. See the current [status](https://github.com/SeasideH1/Matrix-of-Co-Creator/#status).

Obtain the rights required for Minecraft, mods, resources and servers, and comply with applicable Minecraft and component terms. The launcher does not sell or grant Minecraft ownership. File digests verify integrity; use and distribution of content are governed by its license. Check remote addresses and publisher fingerprints; do not distribute content without permission, impersonate another player or bypass service access controls.

### Data and accounts

See the [privacy policy](https://github.com/SeasideH1/Matrix-of-Co-Creator/#privacy-en-us) for recipients, retention and controls. Platform accounts use verified official game identity without a separate platform password. You can export data, remove local credentials or request platform deletion. Deletion has a 30-day cooling period, followed by erasure; minimal security audits last at most 180 days and backups at most 30 days. Recovery within the cooling period requires fresh verification and explicit cancellation. Signing in alone does not restore the account. This is separate from deleting your Microsoft account or game files.

### Updates, recovery and responsibility

This remains alpha software. Signatures verify the release source, and digests verify file integrity; third-party content is governed by its own licenses. Brand migration retains the old installation and local data snapshot. Rollback uses that snapshot; new data is not merged back automatically. Keep usable backups before upgrades or important deletion, and separately handle personal data in retained old copies.

The warranty and liability provisions in AGPL sections 15–17 apply to the extent permitted by law, without excluding rights that cannot legally be excluded. Online services may become unavailable due to maintenance, faults, eligibility or third-party restrictions; permanent availability is not promised. Material behavior/data changes will be disclosed in release notes and policy updates. Public updates are available on the [project home](https://github.com/SeasideH1/Matrix-of-Co-Creator/#project-en-us).

To the fullest extent permitted by applicable law, the operator disclaims all warranties and liability on behalf of Microsoft in connection with this application; rights that cannot lawfully be excluded remain unaffected. Basis: [Microsoft identity platform terms of use, section 2.1.6](https://learn.microsoft.com/en-us/legal/microsoft-identity-platform/terms-of-use).

## License en-US

Project-owned launcher code that the owner has the right to license uses **GNU AGPL-3.0-only**. Use, study, modification, redistribution and commercial use are permitted under that license, including corresponding-source obligations for distribution and modified network services. The complete license, project notice and third-party notices are included in the package.

After installation, corresponding source is located at `resources/source/Matrix-of-Co-Creator-0.1.0-alpha.37-source.zip`, with build instructions at `resources/source/README.build.md`. This archive corresponds to the launcher and does not include the separate main service or game adapter. Source archive SHA-256: `c000d149ce46b10a52b3e39eb134d1253bc1930e29acdd3acb0b24f79b2d476d`.

Third-party code, pre-existing contributions, fonts, images, trademarks, Minecraft, mods and modpacks retain their respective rights. This project does not relicense them or grant additional trademark rights.
