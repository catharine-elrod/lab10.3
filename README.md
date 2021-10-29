
1. See logger.log, why is it different from the log to console?
Logger.log provides the ability to filter information about a log, like level, type, and runtime statistics, so that the messages can later be retrieved and analyzed. 


2. Where does this line come from? FINER org.junit.jupiter.engine.execution.ConditionEvaluator logResult Evaluation of condition [org.junit.jupiter.engine.extension.DisabledCondition] resulted in: ConditionEvaluationResult [enabled = true, reason = '@Disabled is not present']
This line checks to see if a condition or test is disabled or enabled. 

3. What does Assertions.assertThrows do?
AssertThrows is a way to check and see if the test throws an exception of the expected type.

4. See TimerException and there are 3 questions
	1. What is serialVersionUID and why do we need it? (please read on Internet)
	The serialVersionUID is used to keep track of each class by using a unique identifier. We use it to keep track of the compatibility of the serialized object.


	2. Why do we need to override constructors?
	TimerException is a custom exception method that extends Exception. 

	3. Why we did not override other Exception methods?
	The other methods were not made by the user.

5. The Timer.java has a static block static {}, what does it do? (determine when called by debugger)
A static block is a block of code that is only executed the first time a class is loaded into memory.

6. What is README.md file format how is it related to bitbucket? (https://confluence.atlassian.com/bitbucketserver/markdown-syntax-guide-776639995.html)
README.md is a markdown file that is a reference for other users visiting the repo on how to run the project. 

7. Why is the test failing? what do we need to change in Timer? (fix that all tests pass and describe the issue)
The Test Timer Fail tried to keep running after throwing an exception, because the exception was in a Try clause, this lead to a nullPointException happening instead of a TimerException.

8. What is the actual issue here, what is the sequence of Exceptions and handlers (debug)
The exception was in the wrong place, so they program kept running until it reached a different exception.

9. Make a printScreen of your eclipse JUnit5 plugin run (JUnit window at the bottom panel)
Ok.

10. Make a printScreen of your eclipse Maven test run, with console
Ok.

11. What category of Exceptions is TimerException and what is NullPointerException
The NullPointerException is a runtime exception, and the TimerException is a non-runtime exception.

12. Push the updated/fixed source code to your own repository.
ok