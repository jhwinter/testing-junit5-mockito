# Introduction to JUnit 5 with Mockito

All source code examples in the repository are for my [Online Course - Testing Spring Beginner to Guru](https://www.udemy.com/testing-spring-boot-beginner-to-guru/?couponCode=GITHUB_REPO)

This source code repository contains JUnit 5 and Mockito test examples with Maven.

## Setup
### Requirements
* Should use Java 11 or higher. Previous versions of Java are un-tested.
* Use Maven 3.5.2 or higher

## Support
For questions and help:
* Please post in course
* Or post in the Slack Community exclusive to the course.

GitHub Issues will not be addressed.



## Notes

### What is Mockito?

* Mockito is the most popular mocking framework for testing Java
* Mocks (aka Test Doubles) are alternate implementations of objects to replace real objects in tests
* Works well with Dependency Injection
* For the class under test, injected dependencies can be mocks

### Types of Mocks (aka Test Doubles)

* **Dummy** - Object used just to get the code to compile
* **Fake** - An object that has an implementation, but not production ready
* **Stub** - An object with pre-defined answeres to method calls
* **Mock** - An object with pre-defined answers to method calls, and has expectations of executions. Can throw an exception if an unexpected invocation is detected.
* **Spy** - In Mockito, Spies are Mock-like wrappers around the actual object

### Important Terminology

* **Verify** - Used to verify number of times a mocked method has been called
* **Argument Matcher** - Matches arguments passed to Mocked Method & will allow or disallow
* **Argument Captor** - Captures arguments passed to a Mocked Method
  * Allows you to perform assertions of what was passed into the method

### Mockito Annotations

| Annotation   | Description                                 |
|--------------|---------------------------------------------|
| @Mock        | Used to create a mock                       |
| @Spy         | Used to create a spy                        |
| @InjectMocks | Inject mocks / spys into a class under test |
| @Captor      | Captures arguments to Mock                  |
