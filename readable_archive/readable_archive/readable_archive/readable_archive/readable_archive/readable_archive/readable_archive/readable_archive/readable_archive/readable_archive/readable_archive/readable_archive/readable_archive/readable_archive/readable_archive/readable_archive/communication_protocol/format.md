# Format: Ultra-Compressed (Op-Urgency)

## Objective: Maximize Token Density
- **Syntax**: `<ROLE> > <ACTION> | <TARGET> | <STATUS> | <NOTES>`
- **Rule**: Single-line updates preferred. No filler words (the, a, is, are). Use code-style logic symbols.
- **Expert Codes**: `ORCH`, `PLAN`, `SPDP`, `JDP`, `XPM`, `XAD`, `XAA`, `XDM`, `XQA`

## Action Logic
- `->` : input to
- `=>` : results in / leads to
- `@` : targeting / at
- `?` : query / r/o (rule out)
- `!` : urgent / block
- `$` : cost / budget / limit
- `^` : update / deploy / push

## Examples (Military/Medical Hybrid)
- `SPDP > ^ app.py | DEP main => SUCCESS | BC for Liran/Vova ok.`
- `XPM > r/o $ leak @ Food | user:Liran.`
- `XAD > ^ UI @ dashboard | +st.metric | st.progress | style:green.`
- `ORCH > SITREP: All reqs DONE. DEP ^ live.`
