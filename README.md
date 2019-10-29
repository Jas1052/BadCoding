# A Guide to Bad Coding
### How to make your code unreadable, unusable, and unremovable.
---
### Tenants of the Awful Coder
1. **Do not follow any standards.** Rules are for losers and you are not one. If there is a general practice guideline, completely ignore it and be a free spirit. 
2. **Be inconsistent.** Consistency in any shape or letter makes it easy for any developer to eventually figure you out. Roll a dice and toss a coin to determine your next move. Always aim to keep your co-workers on their toes. 
3. **Most importantly, make the code work.** If the code doesn't work, then it becomes tempting to start from scratch and your hard work will be for naught. If the code works but no one can interpret it, then it is inducted into the fabled *legacy code* and no one will dare to change it.
---
#### Naming Conventions
Naming conventions is the bread and butter of the developer since variables act as carriers of information. It is critical to completely make your variables utterely incomprehensible. While many amateurs will simply name their variables or classes `i` or `a`, to confuse other coders, this still makes it easy to understand with enough time and experience. Meanwhile, other malicious developers will make their efforts obvious through garbage values such as `23eli`, which leads to debuggers simply blackboxing the variables and reading through the logic. 

The key to mastering poor naming convention is to create a believable name for a variable, method, or class while sneaking in false information. We can call this technique the **variable entrapment** since the victim will become trapped in a false line of logic. 
Assume the following code:
```
void doSomething(int a, int b) {
    int quotient = obtainQuotient(a, b);
    // proceed with usage of quotient as remainder with no comments
}
```
```
int obtainRemainder(int dividend, int divider) {
    return dividend % divider;
}
```
We apply variable entrapment as such:
```
int obtainQuotient(int divider, int dividend) {
    return divider % dividend;
}
```
It is important to note that the logic is maintained but a developer finds it much more difficult to interpret usage of a falsely named `obtainQuotient(x, y)`, incorrectly thinking that the given code performs as expected. 
