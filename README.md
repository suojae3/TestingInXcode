<br/>


## Testing In Xcode

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

  <br/>

  <img width="546" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/09ea50fc-6ae0-4b9d-a1dd-e679c93f5ccf">

- If you feel like your tests don't fully cover your changes, it may be a good time to go back and write more tests.

<br/>

#

## Test Plans

<img width="851" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/7ae16716-3e11-4161-9c40-f1ea9affaacc">

- test plans allows running your test more than once with different settings.
- as I'm developing my test, I may not run-- run them all those times. So I can choose to just run a single configuration by option clicking on the test diamond and here I see a menu with just so I could select one configuration.
  
<br/>

#

## Continuous Integration Workflows

<img width="491" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/61b61839-53fd-4fe4-93ab-fa2691bf785e">

-   you use the test action, passing in the name of the project and scheme you want to test, as well as the destination on which tests should be run. The second is to build and then test. This puts up the actions of building and testing into two separate invocations of xcodebuild.

<br/>

<img width="882" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/a762b2dc-5f61-45f1-9fa3-606f02d635d2">

- Speaking of running tests, xcodebuild supports testing on multiple devices or simulators at the same time.

<br/>

<img width="659" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/b4e2df23-5158-4d32-ab00-8193515c370e">

- To overwrite the default test plan, use the test plan option passing in the name of the particular plan that you want to run.

<br/>

#

## Result Bundles

<img width="575" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/3cb191e4-a43c-46dc-ab84-b9f1f7308ac0">

- what is a result bundle? A result bundle is a file produced by Xcode containing structured data describing the outcome of building and running your tests.
- The test report showing you which test passed and failed. The code coverage report reviewing which code was covered by the test ran, and any test attachments that were created by the tests using XC test attachment APIs. 

<br/>

<img width="674" alt="image" src="https://github.com/suojae3/TestingInXcode/assets/126137760/c0a3a312-e1cb-40f7-ad5c-622d4dc9eb1b">

- See failing and passing test in the test report, dig into the build failures in the build log, and see how you're doing on coverage in the code coverage report.

<br/>

- Xccov provides programmatic access to the code coverage report either as human readable text or JSON.

