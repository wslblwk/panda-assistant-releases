# 公告资源（announcements 分支）

熊猫助手客户端的公告清单与表情素材。客户端按固定地址读取，请勿删除本分支。

- `announcements.json`：签名后的公告清单（`{ payload, signature }`），由 `node scripts/announcement.cjs --sign` 生成。
- `emojis/`：公告正文里 `[emoji:名字]` 用到的图片，文件名必须与清单 `emojis[].file` 一致。

素材限制：单图 ≤ 48 KiB、边长 ≤ 512px，只支持 png / jpg / webp 静态图（不支持 GIF）。
客户端会按清单里的 SHA-256 校验下载结果，素材被改动需要同时更新清单并重新签名。

更新流程：本地预览 → 用户确认 → 用正式私钥签名 → 提交到本分支（表情图一起放到 `emojis/`）。