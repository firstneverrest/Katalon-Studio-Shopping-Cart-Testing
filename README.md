# Shopping Cart Tests

Navigate to https://docs.katalon.com/katalon-studio/docs/shopping-cart-prj.html for further details.

## Integration with Git

1. Create a repository
2. Click clone git repo in Katalon Studio
3. Fill up git clone url, username and password
4. Select git branch

## Companion products

### Katalon TestOps

[Katalon TestOps](https://analytics.katalon.com) is a web-based application that provides dynamic perspectives and an insightful look at your automation testing data. You can leverage your automation testing data by transforming and visualizing your data; analyzing test results; seamlessly integrating with such tools as Katalon Studio and Jira; maximizing the testing capacity with remote execution.

- Read our [documentation](https://docs.katalon.com/katalon-analytics/docs/overview.html).
- Ask a question on [Forum](https://forum.katalon.com/categories/katalon-analytics).
- Request a new feature on [GitHub](CONTRIBUTING.md).
- Vote for [Popular Feature Requests](https://github.com/katalon-analytics/katalon-analytics/issues?q=is%3Aopen+is%3Aissue+label%3Afeature-request+sort%3Areactions-%2B1-desc).
- File a bug in [GitHub Issues](https://github.com/katalon-analytics/katalon-analytics/issues).

### Katalon Studio

[Katalon Studio](https://www.katalon.com) is a free and complete automation testing solution for Web, Mobile, and API testing with modern methodologies (Data-Driven Testing, TDD/BDD, Page Object Model, etc.) as well as advanced integration (JIRA, qTest, Slack, CI, Katalon TestOps, etc.). Learn more about [Katalon Studio features](https://www.katalon.com/features/).

## How to test with Katalon Studio

### Test Url

- Get Url
- Verify Match

```groovy
WebUI.openBrowser('')

WebUI.navigateToUrl('https://cms.demo.katalon.com/')

WebUI.click(findTestObject('Object Repository/Page_Katalon Shop  Katalon Ecommerce/a_Cart'))

link_cart = WebUI.getUrl()

WebUI.verifyMatch(link_cart, 'https://cms.demo.katalon.com/cart/', false)

WebUI.closeBrowser()

```
