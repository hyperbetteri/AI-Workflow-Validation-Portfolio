# GEH-Core — Research Background and Problems That Remain Open

**Related main document:** [GEH-Core — Public Professional Overview](../portfolio/GEH_CORE_PUBLIC_OVERVIEW_EN.md)  
**Version:** 0.2-EN  
**Date:** September 22, 2026  
**Document timestamp:** 2026-09-22T00:26:01+02:00  
**Author:** Almási Andor Aladár

## 8. Research Background and Problems That Remain Open

The development direction of GEH-Core relates to several problem areas for which artificial intelligence research is still seeking reliable and generally applicable solutions.

The studies below directly document these problems. The references are not independent technical certifications of GEH-Core, but evidence that the problems addressed by the system are real, measurable, and scientifically current.

### 8.1. Weakening of Mandatory Conditions During Agent Handoffs

**When “Must” Becomes “Maybe”: Constraint Weakening in LLM Agent Workflows**  
Direct source: https://arxiv.org/abs/2608.24569

The study examined 1,296 controlled experimental episodes to determine what happens when a mandatory condition identified by one agent passes through summarization, planning, or a handoff to another agent.

The results indicate that the textual content of a condition may be preserved while its mandatory operational force is lost. During normal summary-based handoffs, 100 percent of the examined constraints became deactivated, and prohibited execution occurred in 54.2 percent of cases.

According to the study, semantic preservation alone does not guarantee preservation of operational state.

**GEH-Core connection:**

- preservation of operator intent;
- mandatory state fields;
- context and task-scope protection;
- separate handling of execution conditions;
- fail-closed operation;
- verification of handoff states.

The structured state-management approach of GEH-Core directly addresses this documented problem at the operational level.

Source quality: strong controlled preprint with a large number of experiments; independent replication is still required.

### 8.2. Quality Loss During Task Handoffs Between Different Models

**The Handoff Tax: Continuing Non-Native Trajectories in LLM Agents**  
Direct source: https://arxiv.org/abs/2608.24358

The study examined how performance changes when a long agent workflow is transferred from one language model to another.

The results indicate that switching to a stronger model does not automatically restore quality. Providing the complete previous workflow recovered less than half of the lost performance gap while introducing significant additional cost.

The study demonstrates that model switching is not a neutral operation: the reasoning and workflow trace of the previous engine may constrain the operation of the next engine.

**GEH-Core connection:**

- recording model-handoff state;
- separation of source engine and validation engine;
- structured, minimal state transfer;
- separation of assumptions inherited from the previous engine;
- independent reevaluation;
- detection of handoff distortion.

The multi-model operation of GEH-Core does not assume that mechanical transfer of the complete history preserves the original meaning and quality of the task.

Source quality: comparative preprint covering multiple model families; primarily examined coding agents.

### 8.3. Self-Evaluation Is Not Sufficient to Demonstrate System Improvement

**Aspire: Can Models Self-Evolve from Vague Goals?**  
Direct source: https://arxiv.org/abs/2608.31111

The ASPIRE study examined 520 hidden expert-created tasks to determine whether agents can build their own development and evaluation process from vaguely defined goals.

According to the study, agents frequently selected unsuitable data, relied too heavily on their own narrow evaluations, and local improvements did not carry over to hidden evaluation. Further self-improvement could also erase previously achieved results.

The study indicates that an engine’s own evaluation cannot by itself serve as the final reference.

**GEH-Core connection:**

- no single engine may serve as the exclusive validator of its own operation;
- independent multi-model cross-validation;
- hidden or separated validation tasks;
- regression testing across versions;
- human expert control;
- replayability of previous operational states.

The independent validation layer of GEH-Core is designed directly to reduce bias arising from self-evaluation.

Source quality: preprint based on a large expert-created hidden test set; broader generalizability of the examined goals requires further validation.

### 8.4. Correlated Errors and Misleading Model Confidence

**One Human, N Agents: Audit-Budget Allocation for LLM Agent Fleets under Miscalibrated, Correlated Confidence**  
Direct source: https://arxiv.org/abs/2607.28317

The study examines a situation in which one human must supervise multiple agents under limited audit capacity.

The results indicate that model-generated confidence values were operationally unusable in several cases. The study also found that errors from different model families are not necessarily independent: shared task difficulty may produce stronger correlation than would be expected merely from differences between vendors or model families.

This means that agreement between multiple engines does not by itself prove that an answer is correct.

**GEH-Core connection:**

- no simple majority voting;
- evidence priority;
- examination of error correlation between different engines;
- separate validation of confidence claims;
- targeted use of human review capacity;
- withholding of agreeing but unsupported answers.

GEH-Core cross-validation does not treat model self-evaluation or numerical majority alone as final evidence.

Source quality: preprint combining mathematical and empirical modeling; generalization to real operational environments requires further study.

### 8.5. Lack of Observability and Debugging in Multi-Agent Systems

**Observability and Fault Injection for LLM-Based Multi-Agent Systems in Software Engineering**  
Direct source: https://arxiv.org/abs/2608.24271  
IEEE ICST 2026 publication record: https://doi.org/10.1109/ICST69053.2026.00037

The study begins from the observation that multi-agent systems based on large language models are currently difficult to observe, debug, and examine under controlled failures.

The authors therefore combined unified OpenTelemetry-based tracing with targeted fault injection. The system separately records agent steps, inter-model communication, tool use, and model calls.

The work demonstrates that reproducible tracing and targeted failure analysis remain active areas of development.

**GEH-Core connection:**

- versioned event logging;
- engine-specific decision traces;
- identification of error-propagation points;
- reproducible testing;
- targeted regression testing;
- separation of decision and execution layers.

The event-logging and replay principles of GEH-Core represent a broader multi-model validation approach to the same problem area.

Source quality: technical work published at an IEEE conference; the presented validation currently covers a limited number of systems.

### 8.6. Agent Traces Are Difficult to Audit

**Automata from Agent Traces: Failure and Next-Step Prediction**  
Direct source: https://arxiv.org/abs/2608.23670  
OpenReview record: https://openreview.net/forum?id=1cprFkvFT0

According to the study, long and unstructured agent traces resist traditional safety auditing and runtime monitoring.

The authors constructed finite-state automata from complete traces across twelve public datasets. The extracted state topology enabled early estimation of next steps and expected failures.

One significant result of the research is that observed operational topology may in part be shaped more strongly by the execution framework than by the language model itself.

**GEH-Core connection:**

- separation of model effects from execution-environment effects;
- state-based operational logging;
- detection of drift and router interference;
- early failure indication;
- deterministic replay;
- comparison of multiple runs of the same task.

This supports the conclusion that agent behavior cannot be judged solely from the properties of the underlying model; the external logical and execution system is itself a separate subject of validation.

Source quality: preprint and OpenReview entry based on twelve public datasets; independent reproduction is still required.

### 8.7. Current Benchmarks Do Not Cover Institutional Requirements

**Agent Benchmarks Fail Public Sector Requirements**  
Direct source: https://arxiv.org/abs/2601.20617

The study analyzed more than 1,300 agent benchmarks to determine whether they satisfy procedural, legal, structural, and realism requirements relevant to public-sector environments.

The result was that none of the examined benchmarks satisfied all defined requirements.

This indicates that current general performance measurements alone are insufficient for validating institutional or high-responsibility applications.

**GEH-Core connection:**

- process validation rather than outcome-only measurement;
- logging of decision paths and evidence;
- examination of permission and responsibility layers;
- human approval points;
- validation on real-world workflows;
- domain-specific validation conditions.

The GEH-Core approach examines not only whether the system reached the desired final result, but also through what verifiable process that result was reached.

Source quality: expert-reviewed analysis covering more than 1,300 publications; preprint accepted for conference publication.

### 8.8. Summary Research Conclusion

The cited research independently points in the same general direction:

- model switching can distort a workflow;
- summarization can weaken mandatory conditions;
- an engine’s own evaluation is insufficient;
- errors across multiple models may be correlated;
- majority agreement alone does not constitute proof;
- long agent workflows are difficult to audit;
- the execution environment can significantly shape behavior;
- current benchmarks do not cover all institutional requirements;
- observability and reproducible debugging of multi-agent systems remain open development areas.

The development direction of GEH-Core addresses these problems within a unified operational framework through:

- evidence priority;
- multi-model cross-validation;
- structured state handoff;
- context and task-scope protection;
- ABSTAIN and fail-closed operation;
- human approval and veto authority;
- versioned event logging;
- replayable regression testing.

External research establishes the scientific relevance of the problem domain. Validation of GEH-Core’s own operational results can be provided through documented testing, event logs, reproducible examinations, and later independent professional validation.
