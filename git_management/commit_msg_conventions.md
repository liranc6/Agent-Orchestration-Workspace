<!-- first add your files to the staging area, then run:
git_diff --staged > diffs_output.patch
then write commit message: add both files to agent and write the following prompt: "write a git commit command" or "write a commit msg" -->

Got it! Here’s the updated full guide with your new instructions included about not talking about errors, and structuring the message by stating the purpose first, then what was changed:

---

# GIT: Commit Protocol (Ultra-Dense)
## FMT: `Type: Summary` | `-m Description`
- Description: `PURPOSE -> CHANGES`.
- Key ^ 1 | Key ^ 2 | `file.ext`.
- !ERR: Don't talk about errors.
- DEP: Mention inter-file deps (e.g., `fileB` ^ for `fileA`).

## TYPES
- `Add`: +Feat
- `Fix`: Bug-fix
- `Update`: ^ Improvement
- `Refactor`: restructure (non-functional)
- `Docs`: doc-only
- `Test`: +test | ^ test
- `Chore`: maint (deps/build)

## SHORT-MSG (Small/Low-risk)
- FMT: `Type: Summary`
- USE: cfg ^ | +/- file | sync | rename | doc-only.
- !USE: feat | fix | logic-refactor.

When writing commit messages in the terminal with -m, avoid using backticks (\`) inside double quotes. Use single quotes for multi-line messages or open the editor with `git commit` instead.
Safe approach: use single quotes for the outer -m so you can freely use backticks or single quotes inside:

### Full commit command example:
```
git commit -m 'Add: Integrate HDBSCAN clustering and visualization into ILL evaluation' \
-m 'The primary purpose is to enhance the input loss landscape evaluation by adding HDBSCAN clustering and 2D/3D visualization capabilities to analyze data distributions across forget, retain, and holdout sets for improved interpretability.

The primary changes are:

- Added HDBSCAN clustering functionality in `notbooks/overall_comp.py` with new functions `perform_hdbscan_clustering` and `plot_hdbscan_results`.
- Integrated clustering into the `run_ill_evaluation` function, including PCA and saving of results.
- Updated `evaluate_model_on_benchmark` to save HDBSCAN clusterers and visualizations.
- Modified the `DataManager` class to include a `save_plots` parameter.
- Added necessary imports for PCA, HDBSCAN, and 3D plotting.'
```
