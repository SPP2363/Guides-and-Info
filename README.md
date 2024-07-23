# How to build high quality Software
The topic of how to build mantainable and readable software is a big one in on itself. To get started I want to highlight a few topics to get some inspiration. Coding standards are generally the same for all programming languages. However, each language does have some pecularities. 
One thing, one should be aware of: Good code can be read by anyone not just oneself. In the end this should be the goal.

## Naming Conventions
The first topic is about the naming of variables, classes and every other object in the code. Names should be as descriptive and meaningful as possible. Descriptive names help indentifying the function of the specific object. Even if names get quite long, naming the object after the functionality helps identifying the use.
In case of Python one can refer to the [PEP-8 style guide](https://peps.python.org/pep-0008/).

## Comments
As one probably already know, comments can help understanding the functionality of the code. But not every comment is a good comment. 
A good comprehension is found in [this StackOverflow blog](https://stackoverflow.blog/2021/12/23/best-practices-for-writing-code-comments/):

```
Rule 1: Comments should not duplicate the code.

Rule 2: Good comments do not excuse unclear code.

Rule 3: If you can't write a clear comment, there may be a problem with the code.

Rule 4: Comments should dispel confusion, not cause it.

Rule 5: Explain unidiomatic code in comments.

Rule 6: Provide links to the original source of copied code.

Rule 7: Include links to external references where they will be most helpful.

Rule 8: Add comments when fixing bugs.

Rule 9: Use comments to mark incomplete implementations.
```
If you want to have more information have a look in the blog article

## Version Control
Using a version control system itself does not make good software. But using a version control like Git can help a lot developing good code. Those systems can help getting an overview of the code and structurice programming. 
1. Feature branches:
   When using version control systems you typically have the possibility to create feature branches. Those branches help developing a feature while you still have your stable version on the main branch. This way you can try out new feature no matter the size and complexity and you can always go back to the last stable version. This is especially helpful in continous development but also right at the start. While developing you can create as many branches as you need and you can switch between those without loosing progress or data.
2. Issues:
   In addition to the version control, most tools have features that help keeping the overview. One of those features is an issue board. Those board can be used to create tickets of problems or features that need to be solved or developed. Especially in the context of eiher open source or bigger teams issues help structuring interactions and offer a possibility to contribute without having direct access to the code. 
3. Pull Requests:
   Pull requests is the feature used to merge new code from feature branches to the stable main branch. One good thing about this is to have a good versioning so you always know when a new feature was merged in the main branch and also what files got edited. This way finding bugs gets easier because one can look in the code history. Another reason to use them is the possibility to do code reviews. I will talk about code reviews in the next chapter.

### Code Review
Code reviews are one if not the most important part to ensure good code quality. Since one definition of good code is that others can easily read it, having another person review the code ensures that no errors get into the stable main branch, but also that other people can read it. Pull requests can be an easy tool to accomplish this. When creating a pull request, all the new code is shown in a summary. And only this code is highlighted. This helps to focus on the new code, especially when the code base grows. Another blog who delves deeper in the topic of good and better code reviews can be read [here](https://stackoverflow.blog/2019/09/30/how-to-make-good-code-reviews-better/)

## Modularity
Developing modular code contributes in a few ways on different perspectives to a high quality code. Modularity can be expressed in two ways:
- Encapsulating small code fragments in classes or functions helps minimizing the complexity. Especially in combination with descriptive names of those functions one can understand fast and easily what certain code does. At the same time encapsulating smaller code fragments helps avoiding duplicate code as smaller functions are easier to reuse and recombine.
- At the same time one can use modularity on a bigger scale. Using collections of functions in one module and connecting those modules through linkers help keeping the overview which data is used in which way and where. Linkers control the data which is exchanged from one module to another. This further helps when developing in a group since one can decide on the linkers in the beginning and each developer can program independent of each other. 

## Unit Tests
Unit tests are one of the concepts that help to maintain the code in the long term, especially in larger or more complex projects. Unit tests themselves are tests that are programmed to test the functionality of the smallest units of the program. These units are typically methods that do not call any other self-programmed methods. The aim of a unit test is to check whether the method has the desired behavior and whether this behavior remains the same over the course of development. In this way, you can detect some errors much earlier, even before you try out the program. 
Another way to use unit tests is test-driven development. Before you write the method with the functionality, you can come up with tests that test the desired behavior. Only when you have developed these tests do you start with the actual development of the method. In this way, you have to think in advance about the reason for a function and how it relates to the overall goal.
Unit tests also include very nicely in version control systems and code reviews. Before merging a new feature branch into the main branch one can execute all tests and have a quick look to see if any side effects occur. 
Some more tips for unit tests can be found [here](https://leanylabs.com/blog/good-unit-tests/)

## Stay consistent
One of probably the most important rules is consistency. If you decide on a naming convention or a style, stay with it. Changing conventions only creates confusion if someone does not know the code. Even if you are the only one using the code, you should try to remain consistent. This way you can read the code even if it hasn't been touched for a long time and understand it more easily. After all, you will never know if the code you are writing will be important or even critical in the future, and you need to understand the core structures. Consistency is one of the easiest concepts to apply and helps immensely.

# Further Guides
[Python Cheatsheet](https://github.com/gto76/python-cheatsheet?tab=readme-ov-file)
