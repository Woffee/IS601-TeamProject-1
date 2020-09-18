## Continuous Integration

### What is Continuous Integration?

Continuous Integration (CI) is a development practice where developers integrate code into a shared repository frequently, preferably several times a day. Each integration can then be verified by an automated build and automated tests. While automated testing is not strictly part of CI it is typically implied.

One of the key benefits of integrating regularly is that you can detect errors quickly and locate them more easily. As each change introduced is typically small, pinpointing the specific change that introduced a defect can be done quickly.

In recent years CI has become a best practice for software development and is guided by a set of key principles. Among them are revision control, build automation and automated testing.

Additionally, Continuous Deployment and Continuous Delivery have developed as best-practices for keeping your application deployable at any point or even pushing your main codebase automatically into production whenever new changes are brought into it. This allows your team to move fast while keeping high quality standards that can be checked automatically.

> Continuous Integration doesn’t get rid of bugs, but it does make them dramatically easier to find and remove.

> [Martin Fowler](http://www.thoughtworks.com/continuous-integration?utm_source=Codeship&utm_medium=CI-Guide), Chief Scientist, ThoughtWorks

### Benefits and Advantages of Continuous Integration and Deployment

Continuous Integration has many benefits. A good CI setup speeds up your workflow and encourages the team to push every change without being afraid of breaking anything. There are more benefits to it than just working with a better software release process. Continuous Integration brings great business benefits as well.

#### Reduces Risk

If you test and deploy code more frequently, it will eventually reduce the risk level of the project you are working on as you can detect bugs and code defects earlier. This means they are easier to fix and you can fix them sooner which makes it cheaper to fix them. This will speed up the feedback mechanism and make your communication much smoother, as mentioned in this article by Intercom’s Darragh Curran: [Shipping is your company’s heartbeat](https://blog.intercom.io/shipping-is-your-companys-heartbeat/?utm_source=Codeship&utm_medium=CI-Guide).

#### Better Communication

When you have a CI process in place that is hooked into a Continuous Delivery workflow it’s easy to share your code regularly. This code sharing helps to achieve more visibility and collaboration between team members. Eventually this increases communication speed and efficiency within your organization as everybody is on the same page, always.

#### Faster iterations

As you release code often, the gap between the application in production and the one the developer is working on will be much smaller. Your thinking about how to develop features most probably will change. As every small change will be tested automatically and the whole team can know about these changes you will want to work on small, incremental changes when developing new features. This results in less assumptions as you can build features quicker and test and deploy them automatically for your users to see as soon as possible, thus gaining valuable feedback from them faster.

#### Faster feedback on business decisions

Having a CI process is not only beneficial for software developers, but for their managers as well. Both parties can gather valuable feedback and gain insights much faster. As you push code more often, you have more data available which you can analyze to check if the product is heading into the right direction. This continuous data flow and the timeline of metrics (like dependency, [unit tests](http://blog.codeship.com/behavior-driven-unit-testing-integration-testing/?utm_source=Codeship&utm_medium=CI-Guide&__hstc=753710.ec4cb22c00f2635a21980e0b5dae14b2.1477583947804.1477583947804.1477583947804.1&__hssc=753710.1.1477583947805&__hsfp=4231963282), complexity, and [code smell](https://en.wikipedia.org/wiki/Code_smell)) can also help to reflect on the progress of the project more frequently which enables faster technological and business decisions.

