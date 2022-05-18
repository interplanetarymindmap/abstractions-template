---
prop-name-1612697362: Dependency sorting transform
prop-abstract-1612698044: Given a [[note-1612421759]], it sorts the dependent [[note-1612421759]] based on the work required for them to be curated enough.
prop-is-sensitive-1612698668: false
prop-pir-1643007904: 0.9
prop-transform-1638987875: dependency-sorting
---

Its meant to help to choose what [[note-1612421759]]s to work on in relation to on an intended root-[[note-1612421759]]. It evaluates its [[child-note-1648569735]] dependencies  and gives them a "Required Care Score" based on several metrics. Some intrinsic to the subject note, others based on its [[child-note-1648569735]] dependencies. It tries to optimize for readability and [[semantic-clarity-1646207666]]

- Accuracy:
  [[subject-note-1648569684]] [[prop-pir-1643007904]]
  0 to 1 (float)

- [[transclusivity-1648569157]]:
  Has [[abstraction-pointer-1637564375]]?  Currently only [[prop-name-1612697362]]
  0 or 1 (bool)

- Children [[transclusivity-1648569157]]:
  Average of the Transclusivity score of its dependency [[note-1612421759]]s
  0 to 1 (float)

- Levels
  At what levels down to the root-[[note-1612421759]] nesting tree the [[subject-note-1648569684]] is found
  Array of ints, 0 is root level

- Dilution factor
  Factor applied to each level of the nesting in order to dilute its significance against the root-[[note-1612421759]]
  0 to 1 (float), 0 only root matters, 1 all nesting levels matter equaly

- Completness Score:
  How complete a [[note-1612421759]] Is biased towards [[transclusivity-1648569157]]
  0 to 1 (float). 1 the [[note-1612421759]] is completed, 0 is missing enough stuff to not be opperative.
  Completness Score = Accuracy * [[transclusivity-1648569157]] * Children [[transclusivity-1648569157]]

- Care Required Score: 
  Is the final score given to each [[note-1612421759]] in relation to the root-note. It represents how much "care" the [[child-note-1648569735]] needs in order to make the root-note mor complete
  Care Required Score: Σ level ((1- Completness Score) * DilutionFactor^Level )



Argunents
1. [[subject-note-1648569684]] 
2. [[prop-ipfoam-type-1630602741]] to evaluate. If not defined will evaluate all [[interplanetary-text-1612698201]] properties