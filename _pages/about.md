---
layout: archive
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
I'm Chengran Yang, a fourth-year Ph.D. Candidate at the [School of Computing and Information Systems (SCIS)](), [Singapore Management University (SMU)](https://www.smu.edu.sg), working under the supervision of [Professor David Lo](http://www.mysmu.edu/faculty/davidlo/) (ACM & IEEE Fellow). My research lies at the intersection of **Software Engineering (SE)** and  **Artificial Intelligence (AI)**, focusing on **Harnessing SE Community Knowledge for Developer-Centric Code Intelligence**. My work targets two primary directions:

+ (1) **Improving Code Quality and Security in AI-driven Systems**, specifically focusing on code correctness, runtime efficiency, and vulnerability detection;
+ (2) **Integrating Intelligent Assistants into Developer Workflows**, enabling automated and intelligent support for developer activities, such as automated question answering, documentation generation, and structured code reasoning.

I have 14 publications in top-tier software engineering venues, e.g., ICSE, ASE, TSE, and TOSEM, and received the SMU Presidential Doctoral Fellowship. Before my doctoral studies, I earned my bachelor's degree from the University of Electronic Science and Technology of China (UESTC) and interned at the Institute of Computing Technology, Chinese Academy of Sciences, under the supervision of Prof. Jianfeng Zhan.

## News

+ Jun. 2025 "Think Like Human Developers: Harnessing Community Knowledge for Structured Code Reasoning" got accepted by ICSE 2026
+ Jun. 2025 “APIDocBooster: An Extract-Then-Abstract Framework Leveraging Large Language Models for Augmenting API Documentation" got accepted by ICSME 2025
+ May. 2025 "R2Vul: Learning to Reason about Software Vulnerabilities with Reinforcement Learning and Structured Reasoning Distillation" ranked top-3 most liked papers in the Software Engineering category on the Alphaxiv platform.
+ May. 2025 "ACECode: A Reinforcement Learning Framework for Aligning Code Efficiency and Correctness in Code Language Models" got a major revision by TOSEM

## Lead Contributions (Last 2 Years)

<ul>
  {% assign pubs = site.publications | sort: 'date' | reverse %}
  {% for pub in pubs %}
    {% assign authors = pub.author | split: "," %}
    {% assign first_author = authors[0] | strip %}
    {% assign second_author = authors[1] | strip %}

    {% if first_author contains "Chengran Yang" or second_author contains "Chengran Yang" %}
      <li>
        <strong>{{ pub.title }}</strong><br/>
        {% if pub.author %}
          <em>
            {{ pub.author | replace: "Chengran Yang", "<strong>Chengran Yang</strong>" }}
          </em><br/>
        {% endif %}
        {{ pub.venue }}{% if pub.year %}, {{ pub.year }}{% endif %}
        {% if pub.paperurl %} [<a href="{{ pub.paperurl }}">PDF</a>]{% endif %}
      </li>
    {% endif %}
  {% endfor %}
</ul>

## Service

PC Member:

+ MSR 2023 (junior PC)
+ APSEC2023 (Student Research Competition)

Reviewer:

+ Automated Software Engineering
+ Neurocomputing
+ TOSEM
+ CSAE