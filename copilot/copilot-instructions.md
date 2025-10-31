# Copilot Instructions for fiji-llm

## Local Source Code Access

When you need to understand APIs or implementations not in the current project, search the local source repositories:

```bash
# Search across all repos for a class/method/concept
grep -r "ClassName\|methodName" ~/code/*/*/src --include="*.java" -l

# Search within a specific organization
grep -r "SearchTerm" ~/code/imagej/*/src --include="*.java" -A 5 -B 2

# Find where a class is defined
find ~/code -name "ClassName.java" -type f
```

Source repos are organized as: `~/code/{organization}/{repo}/`
Major organizations: imagej, fiji, scijava, sciview, etc.

The `-l` flag lists files (good for discovery), while `-A 5 -B 2` shows context (good for understanding). Adjust these flags as needed for the task.
