# General
## Info
(X,Y,Z) -> Can be represented as 1, 2, 3 / 1 (For all axes) / 1 X (for specific axis)
### TRANSLATE OFFSET
| Class  | Variant / Default | X, Y, Z |
| :--------: | :-------: | :-------: |
|  TimerClock  | Default | 100 Y |
|  Coin  | Default | 100 Y |
|  CoinRed  | Default | 100 Y |
|  CoinCollect  | Default | 100 Y |
|  BlockTransparent [Editor only] | Default | 50 Y |

### SCALE
| Class  | Variant / Default | X, Y, Z |
| :--------: | :-------: | :-----: |
|  BlockEmpty  | BlockEmpty2x2 | 2 |


### REPLACEMENT
| Class  | Variant / Default | New Model Name |
| :--------: | :-------: | :-------: |
|  TimerClock  | TimerClock100 | TimerClock |
|  TimerClock  | TimerClock10 | TimerClockSmall |
|  BlockHelp  | BlockHelpPatapataWing | BlockHelp |
|  BlockHelp  | BlockAssistAssistItem | BlockAssist |
|  KuriboTower  | Default | Kuribo |
|  PropellerBlock  | Default | BlockPropeller |
|  GeneratorBoxHop  | GeneratorBoxHop | GeneratorBox |
|  GeneratorBoxHop  | GeneratorBoxHopSmall | GeneratorBoxSmall |
|  KillerGenerator  | KillerGenerator | Killer |
|  KillerGenerator  | KillerTailGenerator | KillerTail |
|  KillerGenerator  | KillerMagnumGenerator | KillerMagnum |
|  GororiGenerator  | GororiGenerator | Gorori |
|  GororiGenerator  | GororiBigGenerator | GororiBig |
|  GororiGenerator  | GororiSearchGenerator | GororiSearchGenerator |

### HIDE MESH
| Class  | Variant / Default | Meshes to hide |
| :--------: | :-------: | :-------: |
|  BlockQuestionLong  | Default | BlockQuestionEmpty |
|  Bunbun  | Default | EyelidFull, EyelidHalf |
|  Punpun  | Default | CloseR, CloseL, HalfL, HalfR, QuarterL, QuarterR |
|  Teresa  | Teresa, TeresaTail | TeresaShay |

### ADD MESH
| Class  | Variant / Default | New Model Name | Translation | Rotation | Scale | 
| :--------: | :-------: | :-------: |  :-------: |  :-------: |  :-------: | 
|  PoleGoal  | Default | PoleGoalBall | - |  - |  - | 
|  PoleGoalSuper  | Default | PoleGoalBall | - |  - |  - | 
|  Grass  | All Variants starting with `SnowCover` | SnowCoverGrass | - | - | - |
|  PropellerBlock  | Default | BlockPropellerPropeller | 90 Y | - | - |
|  Wanwan  | Default | WanwanRoot | -100 Y | - | - |

### ANIMATION DEFAULTS
- PresentBox -> wait, color

### SPECIAL
- Pole -> Moves the "Up" Bone by the object's scale  -> `scale.y * 100`

# Arg modifiers

### CHANGE MESHES
#### Tower
| Class  | Variant / Default | Arg Id | RepeatModel | Offset | 
| :--------: | :-------: | :-------: |  :-------: |  :-------: | 
|  SamboHead  | Default | 0 | SamboBody | 115 Y |
|  KuriboTower  | Default | 0 |  KuriboTowerChild | 100 Y | 

#### AddExtraModel
| Class  | Variant / Default | Arg Id | Models | Translation | Scale | Rotation 
| :--------: | :-------: | :-------: |  :-------: |  :-------: |  :-------: |  :-------: | 
|  UpperBlock  | Default | 3| SnowCoverBlock | - | - | - |
|  BlockQuestionLong  | Default | 3| SnowCoverBlockLong | - | - | - |
|  BlockQuestion  | Default | 3| SnowCoverBlock | - | - | - |
|  BlockQuestionFlying| Default | 3| SnowCoverBlock | - | - | - |
|  Kinopio | Default | 5 | BlockPropeller, BlockPropellerPropeller | <0,35,-1.5> <0,135,-1.5> | 1.1 XYZ | - |
|  KinopioTelescope | Default | 5 | BlockPropeller, BlockPropellerPropeller | <0,35,-1.5> <0,135,-1.5> | 1.1 XYZ | - |

#### SwingCoreLength
| Class  | Variant / Default | Arg Id | HeadModel | ChainModel | 
| :--------: | :-------: | :-------: |  :-------: |  :-------: | 
|  SwingSpike  | Default | 3| SwingSpikeHead | SwingSpikeChain |
|  SwingNeedleRoller  | Default | 7 | NeedleRoller | WanwanChain |
|  SwingNeedleRoller  | SwingNeedleRoller8M | 7 | NeedleRoller8M | WanwanChain |

### CHANGE MATERIAL
(plays animation frame -> Sets data to the object/material for that specific frame)
| Class  | Variant / Default | Arg Id | AnimationName | Frame | 
| :--------: | :-------: | :-------: |  :-------: |  :-------: | 
|  Kinopio  | Default | 0 | Color | ArgValue |
|  KinopioRaccoonDog  | Default | 0 |  Color | ArgValue | 
|  KinopioTelescope  | Default | 0 |  Color | ArgValue | 
- Kinopio (telescope raccoondog) -> ArgId = 0, AnimationType = material, AnimationName = Color Frame = argvalue

Material animation -> Material name, affected attribute
