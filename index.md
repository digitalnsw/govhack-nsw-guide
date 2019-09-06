---
layout: sidenav
---
Hello and a very warm welcome to all GovHack participants interested in knowing more about the challenge related to “Rules as Code”. It is a transformational idea that we at the Data, Insights and Transformation branch of NSW Government Department of Customer Service have been working on, over the past several months. As part of the GovHack challenge, our team has put together a short list of things you would need to do in order to set up your own API instance of OpenFisca-NSW. The steps are mentioned below:

1. Create a fork of Openfisca-NSW from [Github ](https://github.com/digitalnsw/openfisca-nsw)
2. Setup an account at [Heroku](https://www.heroku.com/) and create a new app from your Heroku account dashboard.
3. Connect your Github account to the newly created Heroku app.
4. Once the Github account has been linked, search for the forked repository and connect it to the Heroku app.
5. Choose the branch that you wish to deploy, and select the checkbox for “Wait for CI to pass before deploy”, and click on “Enable Automatic Deploys”
6. Select the branch that you wish to deploy and click on “Deploy Branch”
7. Wait a few moments and then click on “Open app”

After following these steps, you should be able to see the following message:

“Welcome - This is the root of an OpenFisca Web API. To learn how to use it, check the general documentation…”

Congratulations – you’ve just set up your own Openfisca Web API.

--------------------------------------------------------------------------------------------------------------------------------------

**Creating your own rules vs utilising pre-existing rules:**

If you are looking to utilise the pre-existing coded rules/rebates/policies, you should use the following from the Openfisca-NSW coded rules:

1. Active Kids
2. Creative Kids
3. NRMA Free 2 Go
4. Family Energy Rebate
5. Gas Rebate
6. National Parks Concessions Pass
7. Teenage Education Payments
8. Disadvantaged Learner Drivers Course
9. StEPS

_It is important to understand that the rules mentioned above are not authoritative in any way, and are experimental in nature._

If you are looking at coding new rules into your forked version of Openfisca-NSW – well, the sky is the limit. Just make sure you add any new “Entities” to your code and incorporate these in tests, if needed. The [Openfisca](https://openfisca.org/en/) website has a lot of documentation and resources that could help you!

**Some more links:**

The coded rules can be found on our Github page: [https://github.com/digitalnsw/openfisca-nsw](https://github.com/digitalnsw/openfisca-nsw)

You can interact with the API/test some of the rules, here: [http://test.nsw.digital/index.html  
](http://test.nsw.digital/index.html)You can have a look at our API Library, here: [http://rules-explorer.herokuapp.com/](http://rules-explorer.herokuapp.com/)

or here: [http://openfisca-nsw-dev.herokuapp.com](http://openfisca-nsw-dev.herokuapp.com)

You can have a look at the react explorer with swagger docs: [http://nsw-rules-dev.herokuapp.com](http://nsw-rules-dev.herokuapp.com)

_It is important to understand that the rules present in the links above are not authoritative in any way, and are experimental in nature._
