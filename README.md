# onboarding-pack 项目上手包

Every project has two sets of knowledge: the written one, and the one in people's heads that takes a month of asking around. This skill writes the second one down.

每个项目都有两套知识：写下来的，和在人脑子里要问一个月的。这个 skill 把第二套写下来。

## Why / 为什么

The expensive onboarding time is never spent on the README's install commands — it is spent discovering the unwritten rules: which file is actually authoritative, which script must never run in prod, why a weird choice was made, who decides what. An agent joining a project (or a human, or you in three months) pays the same tax. The onboarding pack is the tax prepaid, once.

昂贵的上手时间从来不是花在 README 的安装命令上——而是花在发现潜规则上：哪个文件才是权威、哪个脚本绝不能在生产跑、为什么有个怪选择、什么事谁拍板。agent 接手项目（或新人，或三个月后的你自己）交的是同一笔税。上手包就是一次预付。

## The five sections / 五节结构（10 分钟读完）

1. **What & why** — one paragraph: what this is, who it serves, what done looks like.
2. **Run it** — the exact commands, in order, that produce a working setup.
3. **Map** — where things live and which one is authoritative (every project has competing sources of truth; name the winner).
4. **Unwritten rules** — the five or so things that are obvious to insiders and invisible to newcomers ("never edit X directly", "always check Y first", "Z is deprecated but still load-bearing").
5. **Who & where** — owners, decision forums, and where questions go.

## Maintenance rule / 维护规则

The pack is updated **when the thing it describes changes** — a new unwritten rule discovered while working, a file that moved, an owner who changed. Updating it is part of the change, the way tests are: a change that invalidates the pack and does not update it is an incomplete change.

包随其描述的对象变化而更新——工作中发现新的潜规则、文件搬家、负责人变更，更新是变更的一部分，就像测试一样：让包失效却不更新包的变更是不完整的变更。

## Install / 安装

```bash
npx skills add ChenneyZhuang/onboarding-pack
```

Per-agent paths: [COMPATIBILITY.md](COMPATIBILITY.md). MIT. v0.1.0.

各 agent 安装路径见 COMPATIBILITY.md。MIT 许可，v0.1.0。
