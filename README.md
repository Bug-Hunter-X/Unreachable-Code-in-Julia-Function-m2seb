# Unreachable Code in Julia
This repository demonstrates an example of unreachable code in a Julia function.  The `return 0` statement is unreachable because the function always returns a value within the `if-else` block. This could be a minor oversight or a symptom of a larger refactoring issue.  The solution shows how to remove the redundant code for improved clarity and efficiency.

## Bug Description
The bug involves a Julia function containing an `if-else` block where both branches contain `return` statements.  An additional `return` statement outside the `if-else` block is never executed, resulting in unreachable code.

## Solution
The solution removes the unreachable `return 0` statement.