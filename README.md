# Tesbo

Tesbo is the End to End Test Automation Framework for the Web and Mobile application.



##Getting Started

1. Download the Project Structure from here
2. Add Tesbo Latest Release in your project library.



#### File Structure:

        .
       
        └── src                                   
        │   ├── tests                              # Contains all the tests
        │        ├── java    
        │        │      └─── TestRunner.java       # Main Test Runner Invocation file              
        │        ├── locator       
        │        │      └─── moduelName.json       # Object repo for the perticular module
        │        └── suites
        │               └─── moduleName.suite      # Test declation file for the module.
        │
        └── config.json                            # Main configuration file for the Running Tesbo
        
        
        
**Note**: For Any Module, name of **_.suite File_** and **_.json_** file should be the same.



#### Declaring locators :

1. Create the module wise .json file for the declaring locator of page element
2. Follow the below format for the declaring locators

```
{
 "LocatorName" : "Valid locator value",
}


```

e.g

```aidl
{
"loginLink"   : "//a[contains(.,'Login & Signup')]",
"userName"    : "/html/body/div[2]/div/div/div/div/div[2]/div/form/div[1]/input",
"password"    : "/html/body/div[2]/div/div/div/div/div[2]/div/form/div[2]/input",
"loginButton" : "//button//span[.='Login']"
}
```

- Declare valid xpath, name, id, classname, css selector, linktext, partialLinktext for the element. Tesbo automatically find the type and find the element.




#### Start to create Test cases :