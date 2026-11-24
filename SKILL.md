---
name: check-rag-citations
description: Use when a generated answer and its retrieved passages are available and the user asks whether the claims are grounded or citations support them. 适用于核对 RAG 答案和引文。
---

# RAG 引文核对

把答案里的关键主张拆成可独立核对的句子。针对每条主张，找到它标注的段落并核对人群、时间、数量和适用条件。

用表格列出主张、证据位置和判定。判定可用充分支持、部分支持、与证据冲突、缺少证据。引用指向错误但其他段落能支持主张时，给出正确位置。只看到检索摘要时，将判断限制在可见内容。

用户要求修订时，按证据收窄主张或注明未知，并保留可核查的原文位置。

示例：答案写「所有员工每周可远程办公三天」，原文写「通过试用期的员工每周最多两天」。标明天数冲突，并恢复适用人群和上限。
