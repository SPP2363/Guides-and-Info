# How to build good Software
The Topic of how to build mantainable and readable software is a big one in on itself. To get started I want to highlight a few topics to get some inspiration. Coding standards are generally the same for all programming languages. However, each language does have some pecularities. 
One thing, one should be aware of: Good code can be read by anyone not just oneself. In the end this should be the goal.

## Naming Conventions
The first topic is about the naming of variables, classes and every other object in the code. Names should be as descriptive and meaningful as possible. Descriptive names help indentifying the function of the specific obejct. Even if names get quite long, naming the object after the functionality helps identifying the use.
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
Using a version control system itself does not make good software. But using a version control like Git can help a lot developing good code. Those systems can help getting an overview of the code and structure the programming work. 
1. Feature branches:
   When using version control systems you typically have the possibility to create feature branches. Those branches help developing a feature while you still have your stable version on the main branch. This way you can try out new feature no mabgtter the size and complexibility and you can always go back to the last    stable version. This is especially helpful in continous development but also right at the start. While developing you can create as many branches you need. You can switch between those without loosing progress or data.
2. Issues:
   In addition to the version control, most tools have features that help keeping the overview. One of those features is and issue board. Those board can be used to create tickets of problems or features that need to be solved or developed. Especially in the context of eiher open source or bigger teams issues help       structuring inteactions and offer a possibility to contribute without having direct access to the code. 
3. Pull Requests:
   Pull requests is the feature used to merge new code from feature brnaches to the stable main branch. One good thing about this is to have a good versioning so you always know when new features a merged in the main branch and also what files got edited. This way finding bugs gets easier because one can look in the     code history. Another reason to use them is the possibility to do code reviews. I will talk about code reviews in the enxt chapter.

### Code Review
Code reviews are one if not the most important part to ensure good code quality. Since one definition of good code is that others can easily read it, having another person review the code ensures that no errors get into the stable main branch, but also that other people can read it. Pull requests can be an easy tool to accompligh this. When creating a pull request, all the new code is shown in a summary. And only this code is highlighted. This helps to focus on the new code, especially when the code base grows. Another blog who delves deeper in the topic of good and better code revies can be read [here](https://stackoverflow.blog/2019/09/30/how-to-make-good-code-reviews-better/)

## Modularity

## Unit Tests

## Stay consistent

# Further Guides
[Python Cheatsheet](https://github.com/gto76/python-cheatsheet?tab=readme-ov-file)
