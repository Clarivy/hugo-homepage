---
title: "Introduction to CourseBench AI"
url: "/coursebench-ai"
date: 2023-07-23T22:49:07+08:00
draft: false
---
## Why We Need AI Assistance 我们为何需要 AI 的帮助

在面临信息爆炸的时代，``CourseBench`` 专注于为所有学生提供一个公平、独立的课程评价平台。但随着用户数量的增长，我们遇到了一些挑战。各种投诉、举报和学校约谈不仅消耗我们的大量时间和精力，更重要的是，我们坚信每一个声音都应该被听到，每一条评价都有其存在的价值。因此，我们开发了 ``CourseBench AI``，以 AI 的力量来帮助我们实现这个目标。

In the era of information explosion, ``CourseBench`` is committed to providing a fair and independent course review platform for all students. However, as the number of users grows, we face some challenges. Various complaints, reports, and meetings with schools not only consume a lot of our time and energy, but more importantly, we firmly believe that every voice should be heard and every review has its value. Therefore, we developed ``CourseBench AI`` to help us achieve this goal with the power of AI.

## What Are Our Principles 我们的原则是什么 

我们的原则是：公开、透明、独立。我们的目标是，让每一个用户都能在这里自由发表他们的观点，而不需要担心他们的声音被任何人的主观意愿所影响。为了达到这个目标，我们的 ``CourseBench AI`` 遵循以下两个关键原则：

* ``CourseBench AI`` 的处理原则是完全公开透明的。
* 管理员没有权利以任何方式更改/删除/屏蔽用户的评论。

Our principles are: openness, transparency, and independence. Our goal is to allow every user to freely express their opinions here without worrying about their voices being influenced by anyone's subjective will. To achieve this goal, our CourseBench AI follows two key principles:

* The processing principle of CourseBench AI is completely open and transparent.
* The administrator has no right to modify/delete/block user comments in any way.

## How Does CourseBench AI Work CourseBench AI 是如何运作的

``CourseBench AI`` 是我们为了保护用户的言论自由而开发的一个系统。这个系统将所有潜在的违规行为的判断权交由 AI 来处理，确保没有任何人能够侵犯用户的言论自由。

``CourseBench AI`` is a system we developed to protect the freedom of speech of users. This system gives the AI the right to judge all potential violations, ensuring that no one can infringe on the freedom of speech of users. 

``CourseBench AI`` 能自动地根据开源的社区规定来处理任何潜在的违规行为。而 ``CourseBench AI`` 本身也不具有删除评论的权力：它只会在尽可能保证评论中信息量的同时，移除掉违反社区规定的部分。

``CourseBench AI`` can automatically handle any potential violations according to the open-source community regulations. And ``CourseBench AI`` itself does not have the power to delete comments: it will only remove parts that violate community regulations while ensuring as much information as possible in the comments.

在现阶段，由于AI系统尚未成熟以及其高昂成本，``CourseBench AI`` 的行为只能由社区管理员触发。而管理员相比普通用户唯一的额外权力只有：触发 ``CourseBench AI`` 的审查机制。审查机制的已经在开源代码中列出：

- 保留结构良好且具有信息量的信息。
- 在移除冒犯性语言的同时，保留批评性和情感化信息的主要观点。
- 遇到不熟悉的词语或短语时，请删除它们。
- 对含有讽刺或嘲笑性质的信息，只要不包含对教授人格的侮辱，应保持原内容。
- 可以对课程或教学方法发表负面评论，但请避免使用对教授人格的冒犯性词汇。
- **不**改变原文的情感基调。如果原课程评价是负面的，应保持原样。
- 如果内容无意义或只包含冒犯性词汇，需要删除。
- 如果内容与课程或教授的讨论无关，需要删除。
- 进行修改时，需要明确引用社区规定并给出修改原因。

At this stage, due to the immaturity of the AI system and its high cost, the behavior of ``CourseBench AI`` can only be triggered by community administrators. And the only extra power administrators have compared to ordinary users is: to trigger the review mechanism of ``CourseBench AI``. The review mechanism has been listed in the open source code:

- Leave well-structured and informative messages unaltered.
- Preserve the main points of critical and emotive messages while removing offensive language.
- If encountering unfamiliar words or phrases, please delete them.
- For messages containing sarcasm or mocking, maintain the original content as long as it does not include insults directed at a professor's character.
- Negative comments about courses or teaching methods are permissible, but refrain from using offensive words regarding a professor's personality.
- Do **NOT** alter the emotional tone of the original text. If the original review of the course is negative, just retain them.
- If the content is meaningless or only contains offensive words, you need to delete it.
- If the content isn't relevant to discussion about their course or professor, you need to delete it.
- You need to give the reason of your refinement with clear citation to some specific community clauses.

我们的 AI 采用了 ``GPT-4`` 进行推理，其代码已经在 ``GitHub`` 上开源，你可以通过以下链接查看：[CourseBench_GPTWorker/ ↗](https://github.com/Clarivy/CourseBench_GPTWorker/) 。我们相信，通过 ``CourseBench AI`` 的助力，我们可以更好地保护每一个用户的言论自由，让每一个声音都能被听到。

Our AI uses ``GPT-4`` for inference, and its code has been open-sourced on GitHub. You can view it through the following link: [CourseBench_GPTWorker/ ↗](https://github.com/Clarivy/CourseBench_GPTWorker/). We believe that with the help of ``CourseBench AI``, we can better protect the freedom of speech of each user and ensure that every voice can be heard.

