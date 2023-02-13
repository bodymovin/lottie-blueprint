# Blueprint

## Properties  

Definition | Name | Type | Required
-- | :--: | :--: | :--:
[Type](#type) | type | [String](../properties/format-type) | ✅ 
[Title](#title) | title | [String](../properties/prop-types/#string)
[Parser](#parser) | parser | [Parser](./parser/) | ✅ 

## Type

??? Details
    **Property name:** *type*

    **Property type:** [Format type](../properties/format-type)

    **Required**

A unique value to allow the parser validate if the provided json is indeed a blueprint. Its only accepted value is "blueprint"

## Title

??? Details
    **Property name:** *title*

    **Property type:** [String](../properties/prop-types/#string)

A name used to display on the templates list if used within a validation tool.

## Parser

??? Details
    **Property name:** *parser*

    **Property type:** [Parser](./parser)

The parser used for the blueprint.
