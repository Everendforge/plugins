# Everend Plugins

Everend Plugins coordinates runtime adapters for game engines and other execution environments.

Plugins consume Everend runtime packages exported by PathBranching. They should not own canon, replace WorldNotion, or become the primary branching authoring tool.

## Current Status

This repository currently contains roadmap and API documentation only. Engine plugin implementations have not started yet.

## Targets

1. Unity
2. Godot
3. Unreal

## Minimal Runtime API

- Load package
- Start node
- Get current line
- Get choices
- Select choice
- Get/set variables
- Emit events
- Save/load state

## Related Repositories

- [Everend Forge portal](https://github.com/Everendforge/everend-forge)
- [Everend Spec](https://github.com/Everendforge/spec)
- [Everend PathBranching](https://github.com/Everendforge/pathbranching)

## License

Code is licensed under MIT OR Apache-2.0. Documentation is licensed under CC BY 4.0 unless stated otherwise.
