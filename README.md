# Selenium Mobile Emulation Automated (Chrome)
```
# Select which device you want to emulate by uncommenting it
# More information at: https://sites.google.com/a/chromium.org/chromedriver/mobile-emulation
mobile_emulation = {
  "deviceName": "iPhone 6 Plus"
}

# Define a variable to hold all the configurations we want
chrome_options = webdriver.ChromeOptions()

# Add the mobile emulation to the chrome options variable
chrome_options.add_experimental_option("mobileEmulation", mobile_emulation)

# Create driver, pass it the path to the chromedriver file and the special configurations you want to run
self.driver = webdriver.Chrome(executable_path='../driver/chromedriver', chrome_options=chrome_options)
```

### Usage
```
$ python seleniumMobileEmulation.py
```

### Requrements
- Python => 2.7.10
- Selenium webdriver == 3.6.0

#### Note :
- browser = Chrome / chromedriver
- referensi : https://gist.github.com/devinmancuso/ec8ae08fa73402e45bf1
