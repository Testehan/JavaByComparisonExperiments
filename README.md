# Java By Comparison Experiments

“Writing code is easy. Writing good-quality code takes effort, discipline, and a lot of practice. There are many
different definitions for code quality. Here’s mine:
Code Quality
The quality of code is inversely proportional to the amount of effort to understand it.”

“The difference between average programmers and amazing ones is how easy it is for others to follow their work.”


## :fire: Chapter 1 - Start Cleaning Up
Item 1 - Avoid Unnecessary Comparisons.<br>
* “if (microscope.isInorganic(sample) == true)”          BAD
* "if (microscope.isInorganic(sample))"                  GOOD  <br>

Item 2 - Avoid Negations.<br>

Item 3 - Return Boolean Expressions Directly <br>

Item 4 - Simplify Boolean Expressions <br>

Item 5 - Avoid NullPointerException in Conditionals <br>
* “When you validate arguments, you have to mind the order: first check for null and only then for domain-specific
  “illegal” values. We recommend that you check for common default values like empty strings or empty lists
  first, and only then conduct more specific checks.”

Item 6 - Avoid Switch Fallthrough <br>
* “In the rare case where a missing break is intentional, you should leave a comment!”

Item 7 - Always Use Braces <br>
* “Less code is not always better—more readable code is!”

Item 8 - Ensure Code Symmetry <br>
* “The asymmetry in the code came from the fact that we were mixing authorizing code with non-authorizing code.
  We can improve code symmetry if we separate the two into different blocks of code”
*  “First, we handle the unauthorized access, log it, and exit the method. Then, we handle the other two cases
   in an if and a connected else if block.”

## :fire: Chapter 2 - Level Up Your Code Style
“Good code is short, simple, and symmetrical—the challenge is figuring out how to get there.
Sean Parent”

Item 9 - Replace Magic Numbers with Constants.<br>

Item 10 - Favor Enums Over Integer Constants.<br>

Item 11 - Favor For-Each Over For Loops.<br>
* “No need to handle an iteration index anymore! And it even works for arrays and unindexed collections like Set.”
*  “The rare cases where index-based iteration makes sense is when you only iterate over special parts of collections
   or you explicitly need the index for other purposes.”

Item 12 - Avoid Collection Modification During Iteration.<br>
* The solution we’ve depicted here uses another way of iteration: a while loop that relies on the Iterator of our
  supplies collection. The Iterator is our rescue

Item 13 - Avoid Compute-Intense Operations During Iteration.<br>
* If you do something that is compute-intense, it can easily turn into a performance pitfall

Item 14 - Group with New Lines.<br>
*  “As a rule of thumb, you should try to group related code and concepts together and separate different groups
   from each other through empty lines”
* Robert C. Martin uses the metaphor of a newspaper in his book
  Clean Code for describing vertical formatting. A good article starts with the title (class name), goes over
  section headings (public members, constructors, and methods), down to its very details (private methods)

Item 15 - Favor Format Over Concatenation.<br>
* If you have to build large strings, you can use format strings to make them more readable.
* Consider documenting the formatted string with a few examples similar to Document Using Examples so that the
  next developer reading your code doesn’t have to look up how %S or any other special formatting syntax behaves
  to know what the resulting string will be

Item 16 - Favor Java API Over DIY (do it yourself).<br>
* Instead of reimplementing functionality from the API, you should reuse it whenever possible.
  Experts have written and optimized the Java API over time, resulting in a fast and practically bug-free standard
  library
* “Knowing the API well is what makes a true Java professional. You save time if you don’t reimplement (and test)
   functionality that’s already there.”
* The Java API is huge—really huge. In Java 9,
  there are more than 4,000 public API classes alone. Each one of these has a purpose that can help you. We don’t
  recommend that you go through all of them right now. But when you’re programming, ask yourself now and then,
  “Could this piece of code be useful in a different context as well?” If the answer is yes, then there’s a chance
  that you can find a helpful class in the Java API. So you should try searching the API at least briefly.

