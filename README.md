# ECE444-F2022-Lab6

## Unit Test

https://github.com/ECE444-2022Fall/project-1-web-application-design-education-pathways-group-6-lambda/blob/1a496a39e95dab503ae9a5398f43db3a83338d9f/Education_Pathways/tests/test_app.py#L35

## Pros and Cons of Test Driven Development (TDD)

### Pros
- **Test automation**: Automating test cases allows developers to avoid manually testing all features once a new features is added. This is time-efficient, as the alternative is rigorously testing all features via manual testing. Manual testing is prone to human error, making it unreliable on a consistent basis.
- **Security**: Adding unit tests before deployment provides a layer of security against potential logic errors and other functionality bugs developers may have missed. These bugs could be very costly in practice, as it would require extra time and effort to patch these bugs and redeploy. 
- **Modular design**: When making architecture decisions, TDD helps developers break down their programs/services into microfeatures/microservices, that interact with each other. Hence, TDD is a proponent of modular design. 
- **Debugging**: Unit tests explicitly indicate expected behaviours and asserts that expected behaviour is attained. This serves as a debugging tool to indicate flaws in the code that would be difficult to detect by a code reviewer. 
- **Agile**: TDD doesn't disrupt Agile processes and integrates well with CICD processes, serving as a necessary verification step. 

### Cons
- **Time**: TDD at times can be time consuming, nearly doubling the amount of work required for developers. It can seem convoluted for simple features, and can induce stress when trying to meet tight deadlines. It explains why testing is sometimes excluded in startup environments. 
- **QA vs. Dev**: TDD can cause overlap between the role of QAs and developers. TDD encourages developers to write tests and perform quality assurance, reducing the role of QAs. 
- **False confidence**: Unit tests only check for the expected behaviour that the developer specifies. Often times, these test cases are too simplistic, and don't cover edge cases. It is also possible that the developer has specified the expected behaviour incorrectly. TDD can provide a false sense of confidence that code is bug-free, but in reality, more rigorous testing (often manual) is needed.
- **Performance**: TDD is not practical for larger codebases, as just running unit tests can take hours. It is also not ideal if there are limited storage or compute resources.
