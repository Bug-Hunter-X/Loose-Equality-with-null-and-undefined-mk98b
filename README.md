# Loose Equality with null and undefined

This repository demonstrates a common JavaScript error involving loose equality (==) and the handling of null and undefined values.

## The Bug
The `foo` function attempts to check if the input `x` is null and return 0 if so. However, using loose equality (==) with undefined leads to unexpected behavior.  While `null == null` evaluates to true, `null == undefined` also evaluates to true, but `undefined + 1` results in NaN.

## The Solution
The solution replaces loose equality with strict equality (===), which correctly distinguishes between null and undefined values, providing the expected behavior.
