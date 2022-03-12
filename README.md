## MCralwer for java

Web Crawler using Chrome Selenium4   


WebDriverManager.chromedriver().driverVersion("99.0.4844.51").setup();   
ChromeOptions options = new ChromeOptions();   
WebDriver driver = new ChromeDriver(options);   

driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(5));   
driver.manage().timeouts().scriptTimeout(Duration.ofMinutes(2));    
driver.manage().timeouts().pageLoadTimeout(Duration.ofSeconds(10));    

driver.get("https://google.com");    
driver.close();    

