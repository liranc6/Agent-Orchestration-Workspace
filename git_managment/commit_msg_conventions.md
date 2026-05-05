<!-- first add your files to the staging area, then run:
git_diff --staged > diffs_output.patch
then write commit message: add both files to agent and write the following prompt: "write a git commit command" or "write a commit msg" -->

Got it! Here’s the updated full guide with your new instructions included about not talking about errors, and structuring the message by stating the purpose first, then what was changed:

---

# Git Commit Message Guide

## Commit Message Format

Use the following format when creating commit messages (make sure to use the dashes):

git commit -m "Type: Short summary"&#x20; 
-m "Detailed description:

- Key change 1.
- Key change 2.
- Mention functions or files with backticks (\`).
- Keep lines under 100 characters."

## Common Commit Types

- Add: New feature
- Fix: Bug fix
- Update: Minor improvements
- Refactor: Code restructuring without behavior change
- Docs: Documentation only
- Test: Tests added or updated
- Chore: Maintenance tasks (dependencies, build, etc.)

## Guidelines for Describing File Changes

- **Don’t talk about errors.** Avoid describing errors or bugs explicitly in the commit message.

- **State the purpose first, then what you changed.** Begin the detailed description by clearly stating the goal or purpose of the changes, followed by a list of what was actually modified.

- **Mention each file changed:**
  Clearly specify which files were modified in the commit message description. Focus on the purpose or intent behind the changes in each file, rather than listing every function or line altered.

- **Explain inter-file dependencies:**
  If a change in one file requires adjustments in another to maintain compatibility or alignment, explicitly mention this. For example:
  "Modified `fileB.py` to align with changes made in `fileA.py`."

## Example Commit

git commit -m "Refactor: Split input loss landscape evaluation into modular functions"&#x20;
-m "The primary purpose is to modularize loss landscape evaluation for better maintainability.

The primary changes are:

- Extracted logic into `new_ILL_eval`, `get_features`, and `normalize_features` in `loss_landscape.py`.
- Replaced dynamic imports with `sys.path` appends in `utils.py`.
- Added `transformers` to `requirements.txt`.
- Increased UMAP dimensionality from 2 to 10 in `embedding.py`.
- Added AUC heatmap and bar chart of top features in `visualization.py`.
- Modified `plotting.py` to return `matplotlib` figure objects instead of file paths.
- Updated `plotting.py` to align with changes made in `visualization.py`."


## Short Commit Messages

Short commit messages are single-line summaries without a detailed description. Use them when the change is **small, self-explanatory, and low risk**, such as:

* Updating or tweaking configuration files
* Adding or removing a file with a clear purpose
* Syncing submodules
* Minor updates to `.gitignore` or documentation
* Non-functional changes like renaming files or organizing folders

### Format

Follow the same structure as full messages, but only use the first line:

```
Type: Short summary
```

### Examples

```
Chore: Update .gitignore to ignore logs
Docs: Add commit guide
Chore: Sync Unlearn-Simple submodule
Refactor: Rename utils.py to common_utils.py
```

### When **not** to use short messages

Avoid short messages for:

* Feature additions
* Bug fixes
* Refactors affecting logic
* Anything requiring explanation, rationale, or affecting multiple files

In those cases, use a full commit message with a detailed body.

**Note:** 

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
