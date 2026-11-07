# Mandatory engineering rules: original software first

**Original software and languages are the priority, not convenience.**

1. Use original program source, DATA, graphics, control flow, language, interpreter, native compiler/XC and runtime wherever available.
2. Compile complete original-style source through native loading/compilation mechanisms. TERSE screen loading, word definitions, source sequencing, dictionary and target address allocation belong to original TERSE/XC, not a host script.
3. Host scripts may start tools, transport original source unchanged, package native output and independently verify results; never parse TERSE definitions, synthesize dictionaries, assign per-word targets, replace original logic, redraw graphics or rewrite execution tokens.
4. Adapt hardware explicitly in native machine code where required, recording original source and the hardware reason; do not invent logic or visuals in place of existing source.
5. **Hard stop**: investigate and explain any blocked original method, then obtain explicit user approval BEFORE introducing a substitute toolchain/implementation/transformation. Tests passing is no exception.
6. Keep README project/build oriented, sprint plan and technical debt in their named files, and preserve all current work.
7. Report source audits, native builds, ROM comparisons, emulator and hardware execution separately. Never claim unexecuted tests passed or a static scene is complete gameplay.
8. PR acceptance requires original source/toolchain trace, hardware adaptations, documented approvals, actual tests and unresolved work. Reject architectural deviations despite passing tests.

All coding assistants must obey; no self-granted exceptions.
