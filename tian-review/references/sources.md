# 来源与取舍

2026-11-04 根据本会话已检索的公开材料整理。本技能是结合用户偏好和现有技能接口的改写，不是任何原帖的照录；社交平台经验未构成跨模型效果基准。只在追溯来源或更新方法时加载此文件。

| 来源 | 采用的做法 | 未照搬的部分 |
| --- | --- | --- |
| [Reddit：对 AI 代码使用严格审查](https://www.reddit.com/r/ClaudeAI/comments/1ptcbm3/code_quality_of_claude_a_sad_realization/) | 改变生成者视角，检查真实缺陷与遗漏边界；同时保留帖主对误报和过度设计的提醒。 | “讨厌这个实现”的情绪设定、固定复核次数、每轮都应发现问题的暗示。 |
| [Reddit：减少代码审查误报的讨论](https://www.reddit.com/r/claude/comments/1ti1mc3/many_false_positives_in_code_review_using_opus_47/) | 先把疑点当作可证伪的候选，再检查反证，区分确认与未验证。 | 每次固定多代理、强制写报告，以及把模型自评分当作准确率。 |
| [Codex 公开审查规则](https://github.com/openai/codex/blob/main/codex-rs/prompts/templates/review/rubric.md) | 报告具体、可采取行动且有影响的问题，说明触发条件和确实受影响的调用；允许零发现。 | 面向补丁审查的规则只用于变更场景；不套到用户要求的存量模块审查，也不强制使用其 JSON 输出。 |
| [Reddit：方案压力测试提示词](https://www.reddit.com/r/PromptEngineering/comments/1q15mv7/this_is_the_prompt_i_use_when_i_need_chatgpt_to/) | 检查关键假设、现实失败条件和简单可行的替代方法。 | 固定列出三项假设、预设必须反对方案。 |
| [微博：反方、支持方与中立比较](https://weibo.com/2/detail/5333722492838381) | 比较有分量的证据，说明未知变量及结论改变的条件。 | 每次都完整扮演三种角色或强行平衡正反结论。 |

被复用技能的当前本地 `SKILL.md` 才是其流程和适用条件的依据；此处的网络材料只解释入口规则的由来。更新方法时核对原始来源和真实任务表现，优先修正已观察到的问题，保持入口简短。
