# App-Automation-on-EMI-Calculator-with-Appium-Selenium

## Scenario:
     If an user take loan (?) tk from a bank with interest of (?)% and  want to give (?) tk per month as EMI (installment) and processing fee (?)%, 
     how many time period it will take to complete the loan? Take the values from dataset and assert the monthly EMI, total interest, processing 
     fee amount and total payment from the result view. (See below image)

      For solve this question, create a dataset using following values:

      Amount | Interest | EMI | Processing Fee | Monthly EMI | Total Interest | Processing Fee | Total Payment | Period (Year) | Period (Month)

      100000 | 6 | 2000 | 2% | 2000 | 15361.08 | 2000 | 115361.08 | 4 | 10
      200000 | 8 | 5000 | 2% | 5000 | 33391.61 | 4000 | 233391.61 | 3 | 11

      250000 | 7 | 8000 | 1.5% | 8000 | 26804.51 | 3750 | 276804.51 | 2 | 11

      50000 | 10 | 1000 | 5% | 1000 | 14949.12 | 2500 | 64949.12 | 5 | 5
  ## Technology and Tool Used: 
 - Selenium
 - TestNG
 - Appium
 - Android studio
 - Appium inspector
 - Gradle
 - intellij idea
 - Allure
 
 ## How to run this project:
 - clone this project
 - hit the following command into the root directory in terminal:
        - gradle clean test
 - For generating Report in Allure hit the following command
    - allure generate allure-results --clean -o allure-report
 - For view Report in Allure hit the following command
    - allure serve allure-results
    
 - Open Android Studio and Open the APK file:
 - Setup required configuration
 - Start Appium Server with following command: appium -p 4723
 - Open Appium Inspector
 - Set desired capabilites in json format:
 
           {
              "appium:deviceName": "emulator",
              "appium:uuid": "emulator-5554",
              "platformName": "Android",
              "appium:platfromVersion": "11",
              "appium:appPackage": "com.continuum.emi.calculator",
              "appium:appActivity": "com.finance.emicalci.activity.Splash_screnn",
              "appium:app": "D:\\Road to SDET (SQA)\\apk\\emi-calculator.apk"
            }
 ## Prerequisite:
   - JDK 8 or higher
   - Android studio must be installed
   - Appium inspector must be installed
   - Configure GRADLE_HOME and set allure path
   - Start Appium server
 ## Allure Reports:
 ![image](https://user-images.githubusercontent.com/78273243/222914928-1d815c48-4b44-4bd6-8bae-ba698fd220bb.png)
 ![image](https://user-images.githubusercontent.com/78273243/222914951-a28cc256-fa3a-4353-82ac-9cd62dc26073.png)
 ![image](https://user-images.githubusercontent.com/78273243/222915008-d4124f65-f6f4-4e6e-9542-d9db5f1cbed9.png)
 
 ## Gradle Report:
 ![image](https://user-images.githubusercontent.com/78273243/222915058-595999f7-2498-4baf-accc-589c7aee6e0e.png)
 ![image](https://user-images.githubusercontent.com/78273243/222915078-fb6fdc44-ad6f-49d7-91b4-025cf4e560ce.png)


## Video Output: 

https://user-images.githubusercontent.com/78273243/222915216-c726de25-019a-4e1c-97c4-63714e73bc2a.mp4

