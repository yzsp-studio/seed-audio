<div align="center">

# 🎬 seed-audio

## 一句话写场景，人声+环境音+配乐一次生成
## Describe a scene in one line — dialogue, ambience and music in one pass

📮 **商务合作 / Business：wow.vip@foxmail.com**
🎬 **抖音 / Douyin：[v.douyin.com/07EjIDGVErY](https://v.douyin.com/07EjIDGVErY/)**

</div>

---

## 🇨🇳 中文

用自然语言描述直接生成目标音频的技能。描述可以短到一句台词，也可以复杂到多角色对话、环境声、音效与背景音乐组成的完整场景，整段作为一次请求生成，不按角色或场景拆成多次调用再拼接。支持两种模式：T2A 纯文本描述生成，以及 A2A 在描述中引用参考音频指定角色音色。构造请求时把「参考音频 1」「第一个音频」「用某某的」等五花八门的指代归一化为 @音频N，参考列表按首次出现顺序一一对应；用户描述原样保留，不润色、不改写、不翻译、不重排，只剥离与音频内容无关的意图前缀。若主要目标是生成或编辑视频，应改用视频生成或编辑链路。

### ✨ 能做什么

- 一句台词或整段复合场景 → 一次调用直接输出音频结果
- T2A 纯文本描述生成，仅当用户明确指定秒数时才传 duration（1–120）
- A2A 用 @音频1 / @音频2 / @音频3 指定角色音色，参考音频列表 1–3 条且顺序与首次出现一致
- 把「参考音频 1」「第一个音频」「附件 1」「用某文件的」等指代统一归一化为 @音频N
- 多角色对话与多段场景不拆分调用，一次把整段描述传给工具
- 用户描述原样保留，不篡改、不润色、不补全，也不自行添加工具未定义的字段

### 📦 包含的技能

- `seed-audio` —— 见 [`seed-audio/SKILL.md`](seed-audio/SKILL.md)

### 🚀 安装

```bash
git clone https://github.com/yzsp-studio/seed-audio.git
cp -r seed-audio/* "$DSH_HOME/skills/"
```

> 技能是**纯文本说明**（`SKILL.md` + `references/`），零依赖、零 API key，用你当前 agent 的会话额度。

---

## 🇬🇧 English

Generates target audio straight from a natural-language description. The description can be as short as one line of dialogue or as complex as a full scene of multi-character conversation, ambience, sound effects and background music, generated in one request rather than split per character or scene and stitched together. Two modes are supported: T2A from text alone, and A2A where the description cites reference audio to lock a character's timbre. Varied references such as "reference audio 1", "the first audio" or a filename are normalized to @音频N with a 1–3 item reference list matched in first-appearance order. The user's description is passed through untouched — no polishing, rewriting, translating or reordering — with only the non-audio intent prefix stripped. If the real target is video generation or editing, use the video pipeline instead.

### ✨ What it does

- One line of dialogue or a whole composite scene → audio delivered in a single call
- T2A text-only generation; duration (1–120s) is sent only when the user explicitly states a length
- A2A locks character timbre with @音频1 / @音频2 / @音频3, matching a 1–3 item reference list in first-appearance order
- Normalizes varied references — "reference audio 1", "the first audio", "attachment 1", a filename — into @音频N
- Multi-character dialogue and multi-part scenes stay in one call instead of being split and stitched
- The user's description is preserved as written: no rewriting, polishing, completion or extra tool fields

### 📦 Skills included

- `seed-audio` — [`seed-audio/SKILL.md`](seed-audio/SKILL.md)

### 🚀 Install

```bash
git clone https://github.com/yzsp-studio/seed-audio.git
cp -r seed-audio/* "$DSH_HOME/skills/"
```

> Skills are **plain-text instructions** (`SKILL.md` + `references/`). Zero dependencies, no API keys — they run on your agent's existing session quota.

---

## 📮 联系 / Contact

| | |
|---|---|
| 🎬 **抖音 / Douyin** | [https://v.douyin.com/07EjIDGVErY/](https://v.douyin.com/07EjIDGVErY/) |
| 📮 **商务合作 / Business** | **wow.vip@foxmail.com** |
| 🐙 **GitHub** | [https://github.com/yzsp-ai](https://github.com/yzsp-ai) |
| 💖 **打赏 / Support** | [afdian.com/a/yzsp-ai](https://afdian.com/a/yzsp-ai) |

## 📄 License

[MIT](LICENSE) · © 2026 [yzsp-ai](https://github.com/yzsp-ai)
