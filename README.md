# reply-content

回复球 / 输入法的**内容包**。App 通过 raw URL 拉取，改这里不用重新发版。

- `content.json` —— 当前生效的内容包

## 改法

1. 编辑 `content.json`，把 `version` 加 1（必须大于手机上现有的版本号）
2. 提交
3. App 里点「更新内容包」

## 字段

| 字段 | 作用 |
|---|---|
| `prompt.attitude` | 态度层（不跪、给台阶、真诚） |
| `prompt.judge` | 判断层（先判立场/边界，再决定推还是收） |
| `prompt.voice` | 语感层（短、给动作、不解释） |
| `prompt.banned` | 禁词表 |
| `anchors` | 语感锚点，真人会说的话 |
| `cases` | 场景案例，按 `kw` 关键词命中后当参照 |
| `contract` | 输出条数与档位 |

## 署名

案例语料取自 [mouthpieceskill](https://github.com/y1203296842-cloud/mouthpieceskill)（Apache-2.0）。
