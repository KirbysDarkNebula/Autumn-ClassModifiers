### Example Basic file:
`Class.yml`
```yml
Default: // Optional
  ModelReplace: 'ModelName' // Optional
  Translation: // Optional
    X:0
    Y:0
    Z:0
  Scale: // Optional
    X:1
    Y:1
    Z:1
  Rotation: // Optional
    X:0
    Y:0
    Z:0
  HiddenMeshes: // Optional
    - MeshName1
    - MeshName2
  MeshesPriority: // Optional
    MeshName1: Priority // byte
    - MeshName2
  ExtraModels: // Optional
    ExtraModelName1:
      Translation: // Optional
        X: 0
        Y: 100
        Z: 0
      Scale: // Optional
        X:1
        Y:1
        Z:1
      Rotation: // Optional
        X:0
        Y:0
        Z:0
Args:
  TBD
```

The structure seen in  `Default` is a `ModifierEntry`, and we can set a default like that OR add specific entries for different named objects of this class by using `Variants`.
<br> Example:

[BlockHelp.yml](https://github.com/KirbysDarkNebula/Autumn-ClassModifiers/blob/main/Modifiers/BlockHelp.yml)
```yml
Variants:
  BlockAssistAssistItem:
    ModelReplace: 'BlockAssist'
  BlockHelpPatapataWing:
    ModelReplace: 'BlockHelp'
```
