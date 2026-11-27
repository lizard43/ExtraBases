<p align="right"><code>v20261124-0036</code></p>

# Document Host Dev Environment

The [Console 82 - TERSE Glossary](https://github.com/lizard43/dnaTERSE-WB/blob/fe6609fc95b19d8de244761402e51c434c66996d/docs/Console%2082%20-%20TERSE%20Glossary.md) primarily documents target vocabulary and XC bindings. The original host development environment includes additional file management, disk and block management, and source editing vocabulary.

## Vocabulary and execution environment

| Vocabulary | Execution environment |
| --- | --- |
| Standard TERSE | Target cartridge or game runtime |
| Compiler words | Host XC |
| BIOS bindings | Target cartridge |
| File management | Host TERSE |
| Disk and block management | Host TERSE |
| Source editing | Host TERSE |

## Existing evidence

[BOOT-WORDS.md](https://github.com/lizard43/dnaTERSE-WB/blob/fe6609fc95b19d8de244761402e51c434c66996d/docs/BOOT-WORDS.md#L141-L212) and the [Stage 1 Word Registry](https://github.com/lizard43/dnaTERSE-WB/blob/fe6609fc95b19d8de244761402e51c434c66996d/data/word-registry-stage-1.json) document 363 new dictionary headers added during `10 LOAD`, including file management, disk management and source editing words.

| Word | Host execution address |
| --- | --- |
| FINSERT | $3947 |
| B-FINSERT | $3936 |
| A-FINSERT | $3923 |
| -FINSERT | $390E |
| PHYS-INSERT | $3842 |
| DELETE | $31CB |
| INCREASE | $31B3 |
| INSERT | $3186 |
| LOG-PHYS | $30D0 |
| INUSE | $2EE4 |
| FREE | $2ED3 |
| DMAP | $2EA3 |

These addresses are from the Ms. Gorf host dictionary registry. Confirm corresponding bindings directly in the Console 82 host environment and other applicable DNA development environments before documenting their addresses or semantics as verified.

## Glossary expansion

Add three sections to the applicable TERSE glossaries:

- Host File Management
- Host Disk and Block Management
- Host Source Editing

Each entry should include the actual implementation, stack contract, description and cross-references, consistent with the existing glossary format. Distinguish host development vocabulary from target runtime vocabulary and XC bindings. Reconcile against original DNA source and native dictionary evidence.

Apply this research to the Workbench Console 82, Extra Bases, Coloring Book and Cosmic Raiders glossaries. This note records the research task; implementation decoding and native execution verification remain to be completed.
