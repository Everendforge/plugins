# Everend Plugins Roadmap

Everend Plugins are runtime adapters for game engines and other execution environments. They consume runtime packages exported by PathBranching and should not become primary authoring tools.

## Runtime targets

1. Unity.
2. Godot.
3. Unreal.

Unity is the first target because it is the fastest way to validate the full runtime flow.

## Plugin responsibilities

- Import runtime packages.
- Validate references and transitions.
- Execute nodes.
- Expose choices.
- Manage variables.
- Emit events into the engine.
- Save and load runtime state.
- Provide debugging tools in editor/play mode.

## Minimal runtime API

~~~text
LoadPackage(package)
StartNode(nodeId)
GetCurrentLine()
GetChoices()
SelectChoice(choiceId)
GetVariable(name)
SetVariable(name, value)
EmitEvent(eventId, payload)
SaveState()
LoadState(state)
~~~

## Unity prototype

The Unity prototype should:

- Read a JSON runtime package.
- Show current line and choices.
- Select choices.
- Change variables.
- Emit C# events.
- Save and load state.
- Report missing canon references and broken transitions.

## Later split

Once the runtime package is stable, split engine-specific repos:

- unity-plugin
- godot-plugin
- unreal-plugin

Until then, this repository can hold roadmap, examples, and shared adapter decisions.
