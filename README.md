# -Selenium


package testing_practice;     //package 
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
                            //import all required libraries

import org.openqa.selenium.chrome.ChromeDriver;

public class locators_id_xpath{    //class name
	
	public static void main (String[] args) {   //main method
		System.setProperty("webdriver.chrome.driver", "path of chromedriver"); //Setting up chrome using chromedriver by setting its property 
		WebDriver driver= new ChromeDriver() ; //Opening browser
		driver.manage().window().maximize(); //Opening window tab in maximize mode
		  driver.get("https://www.saucedemo.com/");  //Opening application
		  WebElement Location= driver.findElement(By.id("user-name")); //Locate element via ID for Location field and store it in Webelement
		  Location.sendKeys("Testing"); //Input value in Location field
