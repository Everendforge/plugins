# Minimal Runtime API Example

This is the shared conceptual API engine adapters should expose. Names can vary by engine conventions, but behavior should remain compatible.

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
