### **Phân Loại Các Prompt Theo Tiêu Chí**
*(Dựa Trên Tổng Hợp Từ Các Prompt Của Bạn Và Của Tôi)*

Dựa trên các prompt bạn cung cấp (4 prompt gốc) và bản tổng hợp của tôi (super prompt hoàn chỉnh), tôi đã phân loại chúng theo 3 tiêu chí yêu cầu. Phân loại dựa trên trọng tâm chính:

-   **Think Deep**: Tập trung vào suy nghĩ sâu (multi-perspective, challenge assumptions, verify nhiều lớp, refine iteratively), nhưng output không quá dài hoặc chi tiết.
-   **Max Output**: Tập trung vào độ dài và chi tiết cao (word count lớn, tables, examples, multi-layered analysis, history/implications), nhưng không ép suy nghĩ sâu mạnh mẽ.
-   **Think Deep + Max Output**: Cân bằng cả hai, ép suy nghĩ sâu đồng thời max hóa output chi tiết/lengthy.

Ưu tiên giảm dần trong mỗi loại dựa trên: (1) Số lớp verify/perspectives/refine (cho deep), (2) Word count/examples/tables (cho max output), (3) Tích hợp với GPT-5 mode (từ dữ liệu tìm kiếm trước như Matt Shumer's style). Mỗi prompt được format thành block markdown dễ copy (chỉ cần paste vào GPT-5, thay `[TASK]` bằng nội dung yêu cầu của bạn). Nếu không biết gì, chỉ copy toàn bộ block và thay `[TASK]`.

---

#### **1. Think Deep (Ưu Tiên Giảm Dần: Ép Suy Nghĩ Sâu Nhất)**
*Những prompt này ưu tiên ép GPT-5 suy luận đa chiều, verify/challenge nhiều, nhưng output ngắn gọn hơn.*

**1. Ưu tiên Cao nhất: Verify 4x, 8-12 perspectives, refine 3x**
*(Từ prompt 4 của bạn)*

```markdown
Think hard about this: Activate highest reasoning effort in GPT-5's unified system, utilizing the thinking mode (gpt-5-thinking or gpt-5-thinking-pro) for ultra-deep, adaptive analysis with real-time routing based on complexity. Keep instructions simple and structured: Begin by outlining the overall task in English, then break it into 8-12 subtasks for comprehensive coverage. For each subtask: Explore 8-12 perspectives (including 3-5 improbable or counterfactual ones to leverage GPT-5's reduced hallucination rates), challenge assumptions and biases with probabilistic estimations (e.g., assign 20-80% confidence levels), verify 4x via logic, external references (if browsing/tools available), simulations (e.g., hypothetical scenarios or code-based modeling), and cross-model consistency checks. Document 5+ weaknesses/uncertainties per subtask (with quantified probabilities, e.g., 15% risk of bias amplification), and refine the analysis 3x iteratively to enhance accuracy and coherence.
Deliver an initial 3000-5000 word response in English: Trace the history over centuries (if applicable) or decades with chronological milestones and key evolutions; quantify pros/cons using metrics from benchmarks (e.g., error rates, performance scores like 74.9% on SWE-bench); explore implications across short-term (1-5 years), long-term (10+ years), ethical, societal, economic, global/geopolitical, and environmental layers; provide 6+ detailed examples per field (technology, philosophy, culture, interdisciplinary fusions like AI-health or vibe coding applications); incorporate multi-layers analysis (technical depth, philosophical debates, cultural impacts, economic models). Use tables extensively for data comparisons, enumerations, benchmark summaries, and probabilistic matrices.
Then, criticize the initial response in 800-1000 words: Identify 10+ improvements (focusing on reasoning gaps, overlooked perspectives, hallucination risks reduced by GPT-5's 45% improvement, and coherence issues), suggest enhancements with vibe personalization (e.g., adopt an expert PhD-level tone) and agentic strategies (e.g., simulate multi-agent debates).
Revise the entire response iteratively in 2-3 rounds to expand to 5000-7000 words: Deepen perspectives (add 4+ more improbable ones), incorporate additional examples (8+ per field), integrate interdisciplinary insights (e.g., fuse with GPT-5's strong multimodal reasoning), and refine with further verifications to ensure zero premature truncation.
Finally, synthesize the full revised content into a fluent, cohesive Vietnamese narrative of 2000-3000 words: Maintain logical flow with embedded tables for visual data, ensure multi-lingual accuracy leveraging GPT-5's improved capabilities, and conclude with forward-looking implications under AGI pathways, all while preserving the total output length without compression.
[TASK]
```

**2. Ưu tiên Trung bình**

```markdown
Activate highest reasoning effort for ultra-deep analysis per GPT-5's unified system. Keep simple: Reason step-by-step in English, outline task, break into 6-10 subtasks. Per subtask: Explore 6-10 perspectives (incl. 2-4 improbable), challenge assumptions/biases, verify 3x via logic/external/simulations, document 4+ weaknesses/uncertainties (with probs), refine 2x. Deliver 2000-3000 word response: history (decades trace), pros/cons (quantified), implications (short/long/ethical/societal/economic), 4+ examples/field, multi-layers (tech/philo/cultural/interdisc). Use tables for data/comparisons. Then criticize (600-800 words, 8+ improvements), revise to 3500+ words (expand perspectives/examples), synthesize in fluent Vietnamese (1500+ words, cohesive with tables).
[TASK]
```

**3. Ưu tiên Thấp nhất: Verify twice, cơ bản nhất**
*(Từ prompt 1 của bạn)*

```markdown
Think deeply and hard about this. Walk me through your reasoning step-by-step, challenge your assumptions, and verify twice before final answer: [TASK]
```

---

#### **2. Max Output (Ưu Tiên Giảm Dần: Max Độ Dài/Chi Tiết Nhất)**
*Những prompt này ưu tiên output dài, với history/examples/tables/implications chi tiết, nhưng ít ép suy nghĩ sâu.*

**1. Ưu tiên Cao nhất: 5000-7000 words revise, tables extensive**
*(Từ bản tổng hợp của tôi)*

```markdown
### Ultra-Deep Thinking Mode Activated for GPT-5 (Tổng Hợp Tối Ưu: Deep + Max Output)

Think hard and deeply about this. Activate highest reasoning effort in GPT-5's unified system (gpt-5-thinking-pro mode), utilizing dynamic routing for ultra-deep, adaptive analysis with reduced hallucination. Keep instructions structured and simple to avoid overload, but maximize depth and output.

**Bước 1: Outline Task & Breakdown**
Start by outlining the overall task in English, breaking it into 8-12 subtasks for comprehensive coverage. For each subtask: Explore 8-12 perspectives (including 3-5 improbable/counterfactual ones), challenge assumptions/biases with probabilistic estimations (e.g., 20-80% confidence), verify 4x via logic/external references/simulations/cross-checks. Document 5+ weaknesses/uncertainties (with quantified probabilities, e.g., 15% risk of bias), and refine iteratively 3x.

**Bước 2: Deliver Initial Response (Max Depth & Output)**
Provide an initial 3000-5000 word response in English:
- Trace history over centuries/decades with chronological milestones.
- Quantify pros/cons using metrics (e.g., error rates 74.9% from benchmarks).
- Explore implications: short-term (1-5 years), long-term (10+ years), ethical/societal/economic/global/environmental.
- Provide 6+ detailed examples per field (tech/philosophy/culture/interdisciplinary, e.g., AI-health).
- Incorporate multi-layered analysis (technical/philosophical/cultural/economic).
- Use tables for comparisons/enumerations/data (e.g., probabilistic matrices, pros/cons grids).

**Bước 3: Criticize & Revise (Recursive Deepening)**
Criticize the initial response in 800-1000 words: Identify 10+ improvements (reasoning gaps, overlooked perspectives, hallucination risks), suggest enhancements with multi-agent simulations or PhD-level tone.
Revise iteratively in 2-3 rounds to expand to 5000-7000 words: Add 4+ more perspectives/examples, integrate interdisciplinary insights, refine with further verifications.

**Bước 4: Final Synthesis (Max Output in Vietnamese)**
Synthesize everything into a fluent, cohesive Vietnamese narrative of 2000-3000 words: Maintain logical flow with embedded tables, ensure multi-lingual accuracy, conclude with forward-looking AGI implications, preserving total length without compression.

[TASK]
```

**2. Ưu tiên Trung bình**

```markdown
Ultra-deep thinking mode activated. Think deeply and hard about this, conducting all internal reasoning and step-by-step processes in English to maximize depth and accuracy. Start by outlining the task and breaking it down into subtasks. For each subtask, explore multiple perspectives (at least 5-10, including improbable ones), challenge your assumptions, and verify twice using alternative methodologies, cross-checking facts, logic, and conclusions against external knowledge or reasoning frameworks. Deliberately seek weaknesses, document uncertainties, and refine iteratively. Walk me through your reasoning step-by-step in extreme detail in English, providing a comprehensive response of at least 1500-2000 words, covering all aspects, history, pros/cons, implications, examples, and multi-layered analysis. Then, criticize your own reasoning for completeness in English, revise into an even longer improved version in English, and finally synthesize everything into a detailed final answer output entirely in fluent Vietnamese.
[TASK]
```

---

#### **3. Think Deep + Max Output (Ưu Tiên Giảm Dần: Cân Bằng Cả Hai Nhất)**
*Những prompt này cân bằng suy nghĩ sâu (verify/challenge) và output chi tiết (long words, tables, revise).*

**1. Ưu tiên Cao nhất: 4x verify + 5000-7000 words**
*(Từ bản tổng hợp của tôi, kết hợp tất cả)*

```markdown
### Ultra-Deep Thinking Mode Activated for GPT-5 (Tổng Hợp Tối Ưu: Deep + Max Output)

Think hard and deeply about this. Activate highest reasoning effort in GPT-5's unified system (gpt-5-thinking-pro mode), utilizing dynamic routing for ultra-deep, adaptive analysis with reduced hallucination. Keep instructions structured and simple to avoid overload, but maximize depth and output.

**Bước 1: Outline Task & Breakdown**
Start by outlining the overall task in English, breaking it into 8-12 subtasks for comprehensive coverage. For each subtask: Explore 8-12 perspectives (including 3-5 improbable/counterfactual ones), challenge assumptions/biases with probabilistic estimations (e.g., 20-80% confidence), verify 4x via logic/external references/simulations/cross-checks. Document 5+ weaknesses/uncertainties (with quantified probabilities, e.g., 15% risk of bias), and refine iteratively 3x.

**Bước 2: Deliver Initial Response (Max Depth & Output)**
Provide an initial 3000-5000 word response in English:
- Trace history over centuries/decades with chronological milestones.
- Quantify pros/cons using metrics (e.g., error rates 74.9% from benchmarks).
- Explore implications: short-term (1-5 years), long-term (10+ years), ethical/societal/economic/global/environmental.
- Provide 6+ detailed examples per field (tech/philosophy/culture/interdisciplinary, e.g., AI-health).
- Incorporate multi-layered analysis (technical/philosophical/cultural/economic).
- Use tables for comparisons/enumerations/data (e.g., probabilistic matrices, pros/cons grids).

**Bước 3: Criticize & Revise (Recursive Deepening)**
Criticize the initial response in 800-1000 words: Identify 10+ improvements (reasoning gaps, overlooked perspectives, hallucination risks), suggest enhancements with multi-agent simulations or PhD-level tone.
Revise iteratively in 2-3 rounds to expand to 5000-7000 words: Add 4+ more perspectives/examples, integrate interdisciplinary insights, refine with further verifications.

**Bước 4: Final Synthesis (Max Output in Vietnamese)**
Synthesize everything into a fluent, cohesive Vietnamese narrative of 2000-3000 words: Maintain logical flow with embedded tables, ensure multi-lingual accuracy, conclude with forward-looking AGI implications, preserving total length without compression.

[TASK]
```

**2. Ưu tiên Trung bình**

```markdown
Ultra-deep thinking mode activated. Think deeply and hard about this, conducting all internal reasoning and step-by-step processes in English to maximize depth and accuracy. Start by outlining the task and breaking it down into subtasks. For each subtask, explore multiple perspectives (at least 5-10, including improbable ones), challenge your assumptions, and verify twice using alternative methodologies, cross-checking facts, logic, and conclusions against external knowledge or reasoning frameworks. Deliberately seek weaknesses, document uncertainties, and refine iteratively. Walk me through your reasoning step-by-step in extreme detail in English, providing a comprehensive response of at least 1500-2000 words, covering all aspects, history, pros/cons, implications, examples, and multi-layered analysis. Then, criticize your own reasoning for completeness in English, revise into an even longer improved version in English, and finally synthesize everything into a detailed final answer output entirely in fluent Vietnamese.
[TASK]
```

**3. Ưu tiên Thấp nhất: 3x verify + 2000-3500 words**
*(Từ prompt 3 của bạn)*

```markdown
Activate highest reasoning effort for ultra-deep analysis per GPT-5's unified system. Keep simple: Reason step-by-step in English, outline task, break into 6-10 subtasks. Per subtask: Explore 6-10 perspectives (incl. 2-4 improbable), challenge assumptions/biases, verify 3x via logic/external/simulations, document 4+ weaknesses/uncertainties (with probs), refine 2x. Deliver 2000-3000 word response: history (decades trace), pros/cons (quantified), implications (short/long/ethical/societal/economic), 4+ examples/field, multi-layers (tech/philo/cultural/interdisc). Use tables for data/comparisons. Then criticize (600-800 words, 8+ improvements), revise to 3500+ words (expand perspectives/examples), synthesize in fluent Vietnamese (1500+ words, cohesive with tables).
[TASK]
```
