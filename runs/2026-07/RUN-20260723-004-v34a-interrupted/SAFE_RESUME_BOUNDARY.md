# Safe resume boundary

Current status: `SAFE_RESUME_CONDITIONAL_ON_TARGETED_NPZ_LOAD_TEST`.

Recheck seven representation families, batches 1?76, and absence of 77. Before unconditional resume, use an already-installed scipy environment to read-only load-test each family?s batches 1 and 76 plus risk batches 1 and 2. No existing scipy environment was found in this audit. ZIP central-directory checks, continuity, zero-byte checks, and risk-size audit all pass.

After targeted load tests pass, resume only `build_fulltext_representations_v3_4a.py` from batch **77**. Do not overwrite 1?76. Topic, residual, finalizer, and CHAT_UPLOAD_PACK remain forbidden until all 1?92 batches and an explicit representation checkpoint are validated. Route B remains `TERMINATED_DO_NOT_REVIVE`.
