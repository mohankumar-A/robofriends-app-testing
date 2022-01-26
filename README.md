# robofriends-testing

To run the project: 

1. Clone this repo
2. Run `npm install`
3. Run `npm start`
4. Run tests with `npm test` -- you may have to press "a" to run all tests

HEADS UP! Depending on your version of Jest, you may find that your snapshots aren't created properly (empty). This is a known issue and may require you to do the following: https://backbencher.dev/blog/empty-shallowwrapper-snapshot-jest-enzyme. I have included the code change mentioned in the article in this git repo to show you how to do this if you encounter the issue.

# Testing:

TDD: test driven development

- Unit test (indivual functinality)
    all small pure functions.
    it wont test contract between two.
    easy to implement.
- Integration test (merge differnt functionalities)
    all about cross communication.
    spies, mocking libraries to assert.
    stub to modify the testing.
    can test connection/contract between the functionalities.
    harder to write.
- Automation test (manually test real case scenorias, etc)
    UI test
    user behaviour test
    takes longer time
    nigtmare (web scarp etc), testcafe (simple without cross browser), cypress, webdriver.io (best documentation)
    manual tester will do this work
    takes more time (depends on company and work environment)
## testing tools:

- testing library (scaffolding)
    Jasmine, Jest, mocha
- assertion library (essentially will)
    Jasmine, Jest, Chai with Mocha
- test runner
    Jasmine, Jest, Mocha, Karma.js
    DOM, puppeteer, jsdom
- mock, spies and studs
    Jasmine, Jest, sinon.js
- code coverage:
    istanbul, jest with running under istanbul

snapshot testing, enzyme

## Asynchronous test

Jest:

 - use async await
 - done
 - return

## cheat sheet

Moving forward, you should use the [Jest Cheat](https://github.com/sapegin/jest-cheat-sheet) Sheet to help you along as you write tests if you are coding along in the videos. It will also come in handy at the end of this course where you will have to write tests for our robofriends app. 

## mocks and spies:
mocks: fake the api and behviour of the function

## enzyme:

- shallow - only the main component rendering, not the child components
- mount - full DOM rendering
- render - 

To learn more about the 3 techniques used in Enzyme for testing: shallow, mount, render, have a look at their [api documentation](https://enzymejs.github.io/enzyme/docs/api/) to see what kind of methods you can use to test your components. We will be using some of them in the later parts of this section.

Depending on your version of Jest, you may find that your snapshots aren't created properly (empty). This is a known issue with Jest and may require you to do the following: https://backbencher.dev/blog/empty-shallowwrapper-snapshot-jest-enzyme. I have included the code change mentioned in the article in this git repo to show you how to do this if you encounter the issue.

nock library for async testing
supertest library for async testing

## Exercise: #5 - Final Tests
Using this [Github repo](https://github.com/aneagoie/robofriends-testing) which contains the tests you saw in my videos for the robofriends app, continue to practice and add your own tests and see if you can improve the code coverage. Use this as a playground to try different packages, techniques, and methods that you want so you can improve your skill and be comfortable with testing. Share your coverage report in the #juniortosenior Discord channel to show off once you are done :)

## Note: What Test is Best?
As always, you should always consider asking why and challenging common assumptions and make the decisions that make sense for a specific project. Here is an excellent article that argues an uncommon opinion when it comes to testing, with valid points: https://blog.usejournal.com/lean-testing-or-why-unit-tests-are-worse-than-you-think-b6500139a009