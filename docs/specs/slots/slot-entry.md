# Slot Entry

## Properties  

Definition | Name | Type | Required
-- | :--: | :--: | :--:
[Name](#name) | name | [String](../../../properties/format-type) | ✅ 
[Type](#type) | type | [Validation type](../../../properties/validation-type) 
[Count](#count) | count | [Count](../../../properties/count)

## Name

??? Details
    **Property name:** *name*

    **Property type:** [String](../../../properties/format-type)

The name of the slot that needs to be validated. If the json doesn't have any slot that matches this rule name combined with the count rule, an error will be appended to the error list.

## Type

??? Details
    **Property name:** *type*

    **Property type:** [Validation type](../../../properties/validation-type

The type of pattern matching that will be applied to the rule. It accepts either "regex" or "string".

## Count

??? Details
    **Property name:** *count*

    **Property type:** [Count](../../../properties/count

The type of comparison that will be applied to validate whether the animation matches the number of occurrences. 