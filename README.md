# A Guide to Bad Coding
### How to make your code unreadable, unusable, and unremovable.
---
### Tenants of the Awful Coder
1. **Do not follow any standards.** Rules are for losers and you are not one. If there is a general practice guideline, completely ignore it and be a free spirit. 
2. **Be inconsistent.** Consistency in any shape or letter makes it easy for any developer to eventually figure you out. Roll a dice and toss a coin to determine your next move. Always aim to keep your co-workers on their toes. 
3. **Most importantly, make the code work.** If the code doesn't work, then it becomes tempting to start from scratch and your hard work will be for naught. If the code works but no one can interpret it, then it is inducted into the fabled *legacy code* and no one will dare to change it.
---
### Why should you follow this guide when coding?
Imagine a scenario where you are using this guide to do your work for some company. One day, the company has an ill-conceived notion that it might be possible to replace you with new talent. After all, it's possible that the fresh, young developer may be able to do your job better. At first, your co-workers are relieved to finally escape your onslaught of appaling code and illegible codebase. But they soon come to realize that although you produce garbage, this garbage is the foundation of the product and they will be the forsaken ones left to maintain it. It becomes clear, someone else less essential will need to go. One by one, you see them leave, defeated by the ebb and flow of the corporate environment. Eventually, you become the sole employee to understand any of the horrifying codebase, emboldened by years of survival and attrition. Before anyone realizes, the company now relies on your existance to survive. You have become the vestigial organ that cannot be cut off. Welcome to our guide.

---
#### Naming Conventions
Naming conventions is the bread and butter of the developer since variables act as carriers of information. It is critical to completely make your variables utterly incomprehensible. While many amateurs will simply name their variables or classes `i` or `a`, to confuse other coders, this still makes it easy to understand with enough time and experience. Meanwhile, other malicious developers will make their efforts obvious through garbage values such as `23eli`, which leads to debuggers simply blackboxing the variables and reading through the logic. 

The key to mastering poor naming convention is to create a believable name for a variable, method, or class while sneaking in false information. We can call this technique **variable entrapment** since victims become trapped in a false line of logic. 
Assume the following code:
```
void doSomething(int a, int b) {
    int remainder = obtainRemainder(a, b);
    // proceed with usage of remainder with no comments
}
```
```
int obtainRemainder(int dividend, int divider) {
    return dividend % divider;
}
```
We apply variable entrapment as such:
```
void operation(int a, int b) {
    int quotient = obtainQuotient(a, b);
    // proceed with usage of quotient as remainder with no comments
}
```
```
int obtainQuotient(int divider, int dividend) {
    return divider % dividend;
}
```
It is important to note that the logic is maintained but a developer finds it much more difficult to interpret usage of a falsely named `obtainQuotient(x, y)`, creating incorrect assumptions about a block of code.

Another set of powerful tools for the awful coder is ***V A G U E N E S S*** and repetition. Usage together expontentially makes code more difficult to read and will leave people with their head's scratching. 

For example, if we have a set of summation tools, we can fail to name them:
```
int math(int a, int b) {
    return a + b;
}
int lessMath(int a, int b) {
    return a + b - 1;
}
int math1(int a, int b) {
    return a**b;
}
int mathmath(int a) {
    return a + a;
}
```
The next reader, without delving into each method, will be left scratching their head and saying "What is the difference between any of these?" While this question can be answered by reading through every line in every method, this technique used in succession can incapacitate the developer's ability to debug and requires complete understanding of code in combination with patience beyond human capability. 

#### Spacing
#### Comments
#### Functions and Method Organization
#### Organization of Codebase
### Constants File
