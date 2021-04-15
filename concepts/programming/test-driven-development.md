# Test-driven development

### Why test-driven \(testing-first\) development?

In **test-driven development \(TDD\)**, we would write tests before the code \(instead of after\), doing such:

* creates a natural documentation - an outline - of the program that we will write
* ensures testing infrastructure from the get-go 
  * writing program code first tends to shy away from writing testing code later
    * \(especially if "it works"\) 
* allows us to test incrementally and focus on modular functionality
* motivates us to refactor and write cleaner program code

### Test-driven development cycle

1. write test code
2. run test code \(it should fail\)
3. write program code
4. run test code \(it should pass\)
5. if it passes, refactor program code 
6. repeat

### Test code anatomy

* `describe` a user story 
  * `it` should expect some outcome based on
    * some programatically-automated operations
  * it will `assert` the equality, inclusion or some other quality in order to pass the test



