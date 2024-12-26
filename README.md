# JavaScript Loose Equality Bug

This repository demonstrates a common JavaScript error related to loose equality (==) and the handling of null and undefined values. The `foo` function is intended to add two numbers, but its behavior is unpredictable when one or both inputs are null or undefined.

## Problem

The original `foo` function uses loose equality (===) to check for null values.  Loose equality can cause unexpected type coercion, leading to logical errors.  For example, `0 == false` is true, even though they aren't the same type.

## Solution

The solution involves using strict equality (===) to test for null or undefined values. This ensures that type checking is performed, and we have more predictable behavior. Additionally, it incorporates explicit checks for undefined values. 