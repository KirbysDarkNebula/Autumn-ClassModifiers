# General
### TRANSLATE OFFSET
- TimerClock(100 / 10) ->  100 Y
- Coin CoinRed -> 100 Y
- CoinCollect ->  100 Y

### SCALE
- BlockEmpty2x2 -> scale = 2

### REPLACEMENT
- TimerClock100 -> TimerClock
- TimerClock10 -> TimerClockSmall
- BlockHelpPatapataWing -> BlockHelp
- BlockAssistAssistItem -> BlockAssist

### HIDE MESH
- BlockQuestionLong HideMeshes -> BlockQuestionEmpty
- Bunbun HideMeshes -> EyelidFull, EyelidHalf
- Punpun HideMeshes -> CloseR CloseL HalfL HalfR QuarterL QuarterR

### ADD MESH
- PoleGoal (Last) -> PoleGoalBall
- PoleGoalSuper -> PoleGoalBall

### ANIMATION DEFAULTS
- PresentBox -> wait, color

### SPECIAL
- Pole -> Moves the "Up" Bone by the object's scale  -> `scale.y * 100`

# Arg modifiers

### CHANGE MESHES
- SamboHead AddParts -> ArgId = 0, RepeatModel = SamboBody, Offset = vec3 (115 Y)
- KuriboTower AddParts -> ArgId = 0, RepeatModel = null (repeats), Offset = vec3

## CHANGE MATERIAL
(plays animation frame -> Sets data to the object/material for that specific frame)
- Kinopio (telescope raccoondog) -> ArgId = 0, AnimationType = material, AnimationName = Color Frame = argvalue

Material animation -> Material name, affected attribute
