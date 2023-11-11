# TestingInXcode



<br/>


<img width="667" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/62d883d7-dd45-42b9-a3fb-ef85b0e0ad87">

- Unit tests are the foundation of pyramid.
- Unit tests help verify a single piece of code, generally a function.
- Next is integration tests. it validate a larger section of your code. 
- Integration tests should target discrete subsystems or clusters of classes to make sure that different components behave correctly together.
- Integration test is part of unit test, because you want to make sure that the individual function behave correctly before testing larger pieces of your code.
- Lastly User-Interface Tests observe the user-phasing behavior of your app.

<br/>

<img width="823" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/87c728a0-35bd-40dc-8420-2904751bb249">

- Performance tests run mmultiple times over a given test to look at the average timing, memory usage or other metric.

<br/>

<img width="684" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/ce4bfd4a-f6c6-42cf-9853-89f07d999c48">

- XCTAssertEqual will compare the first two values given to it and make sure that they're equal. If they differ, the test will fail instead.

<br/>

<img width="651" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/60efb045-ff92-4475-98ae-fcf28fb73748">

<br/>

- These blocks serve as a way for you to do any work you need to around your test in order to keep your tests specific to their purpose. SetUp is called before each of your test cases executes. In UI test, this helps ensure that your app is launched before you try interacting with it.

<img width="599" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/37a8c3a5-81e7-4d80-aa4f-15ddc22ce39e">

- So, I can add an accuracy argument instead of equal to one. This will allow XCTAssertEqual to have a leniency and allow the numbers to defer by one and still pass the test.

<br/>

<img width="613" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/62f34d06-b820-403d-a90e-82f39dd7f504">

- The next function I'm going to write is going to be a negative test case.
-  I'll expect an error to be thrown to say that the city is unknown in our database. I can use XCTAssertThrowsError to do this


<br/>

<img width="472" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/ceb13227-be6b-4c63-bc61-4a056b6e17a2">

- IsHittable will ensure both that the element exists and that is on the screen so we can interact with it. 

<br/>

<img width="642" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/7b8584ae-9f01-4557-81ca-904cd9b4cc5b">

- when starting to write your test class, you'll start out with two test targets, generally, one for unit tests and one for UI tests.
- Each of these test classes-- test targets will contain your test classes.
- Your test classes then contain each of your test cases.

<br/>

<img width="644" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/ae05eed3-bd2f-429a-92b3-510e50c226a9">

- Code Coverage is a feature in Xcode in XCTest that will measure and visualize the number of times each line of your source code was executed during your test run.
- You can also see complex information showing individual code paths that were not hit during your test, such as conditionals that were never selected.

