## Example showing usage of extentreports-cucumber4-adapter

The example is from the official Cucumber project.

### How to

Steps you need to follow to use the extentreports adapter for Cucumber JVM:

* Start with marking your runner with the adapter [link](https://github.com/foursyth/extentreports-cucumber4-example/blob/master/src/test/java/cucumber/examples/java/calculator/RunCukesTest.java):

```
@RunWith(Cucumber.class)
@CucumberOptions(plugin = {"com.aventstack.extentreports.cucumber.adapter.ExtentCucumberAdapter:", "json:target/cucumber-report.json"})
@Category(Example.class)
public class RunCukesTest {
}
```

* Now, to tell the adapter which reporters you will be using, add `extent.properties` under `src/test/resources/` [link](https://github.com/foursyth/extentreports-cucumber4-example/blob/master/src/test/resources/extent.properties)
