# FLOW: Op-Urgency Process
1. INTAKE: @user_requests -> XPM/SPRD read mission | !CLEAR -> Q? user.
2. CLARIFY: XPM + XAA + SPDP + XAD review | r/o assumptions/risks | !CLEAR -> Q? user + REC.
3. SYNC: ^ msgs/YYYYMMDD-<topic>/README.md thread | SPDP/JDP alignment | devs Q? -> XPM | !STALL.
4. PLAN: PLAN -> def tasks | ^ specs | assign task:DEV | def DONE.
5. BUILD: DEV -> WIP only after msgs/ thread exists and reflects plan | !BLOCK -> reason | Q? msgs | req ^ -> goto 2.
6. VERIF: XCR review (PR#) | XQA test (TF/TP) | TF -> goto 5.
7. DLVR: TP => DONE | XPM/XDM release | FYI: delivered.
8. ARCH: DONE -> archive/ | !CLEAN folders.
