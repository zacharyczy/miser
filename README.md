# miser

一个用于 Codex 的任务分流 Skill：在用户要求多模型协作时，帮助 Astra 主代理判断哪些明确、独立的子任务适合交给其他模型，并保留主代理对目标、边界和验收的负责。

A Codex skill for assigning bounded, independent subtasks across models when the user asks for multi-model collaboration. The Astra lead keeps responsibility for scope, review, and delivery.

## 使用

将本目录放入 Codex 的技能目录，按 Codex 的技能机制加载。完整规则见 [SKILL.md](SKILL.md)。需要时可明确提出“使用 $miser”。

这个 Skill 只提供任务分流规则；它不切换当前模型，也不安装或解锁其他模型。
