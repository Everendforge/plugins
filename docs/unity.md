# Unity Adapter Notes

Unity is the first planned runtime target.

## Prototype goals

- Import an Everend runtime package JSON file.
- Start a node by ID.
- Read current line data.
- List available choices.
- Select a choice and advance state.
- Get and set variables.
- Emit C# events.
- Save and load runtime state.
- Report missing canon references and broken graph transitions.

## Non-goals

- No graph authoring inside Unity for the first prototype.
- No canon editing inside Unity.
- No dependency on WorldNotion or PathBranching at runtime.
