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

### HIDE MESH
| Class  | Variant / Default | Meshes to hide |
| :--------: | :-------: | :-------: |
|  BlockQuestionLong  | Default | BlockQuestionEmpty |
|  Bunbun  | Default | EyelidFull, EyelidHalf |
|  Punpun  | Default | CloseR, CloseL, HalfL, HalfR, QuarterL, QuarterR |

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
#### "Tower"
| Class  | Variant / Default | Arg Id | RepeatModel | Offset | 
| :--------: | :-------: | :-------: |  :-------: |  :-------: | 
|  SamboHead  | Default | 0 | SamboBody | 115 Y |
|  KuriboTower  | Default | 0 |  Kuribo / same as KuriboTower | 100 Y | 
#### ExtraParts
| Class  | Variant / Default | Arg Id | ExtraModel | Offset | 
| :--------: | :-------: | :-------: |  :-------: |  :-------: | 
|  UpperBlock  | Default | 3| SnowCoverBlock | - |
|  BlockQuestionLong  | Default | 3| SnowCoverBlockLong | - |
|  BlockQuestion  | Default | 3| SnowCoverBloc | - |
|  BlockQuestionFlying| Default | 3| SnowCoverBloc | - |

### CHANGE MATERIAL
(plays animation frame -> Sets data to the object/material for that specific frame)
| Class  | Variant / Default | Arg Id | AnimationName | Frame | 
| :--------: | :-------: | :-------: |  :-------: |  :-------: | 
|  Kinopio  | Default | 0 | Color | ArgValue |
|  KinopioRaccoonDog  | Default | 0 |  Color | ArgValue | 
|  KinopioTelescope  | Default | 0 |  Color | ArgValue | 
- Kinopio (telescope raccoondog) -> ArgId = 0, AnimationType = material, AnimationName = Color Frame = argvalue

Material animation -> Material name, affected attribute
