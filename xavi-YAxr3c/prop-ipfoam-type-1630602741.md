---
prop-ipfoam-type-1630602741:
  defaultName: TypeDefinition
  represents: Type to defines other types.
  constrains:
    - Not in use. Currently hard-coded as its the origin for validating types itself
  ipldSchema: >
    type root struct {
        defaultName defaultName
        represents represents
        constrains  optional constrains
        typeDependencies optional typeDependencies
        ipldSchema ipldSchema
    }   

    type defaultName string
    type represents string
    type constrains [string]
    type typeDependencies [string]
    type ipldSchema string
---