package seleniumlearn;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.annotations.Test;

public class seleniumlearn {

    @Test
    public void myTest() {
    	String username = "admin";
    	String password = "admin";
        System.setProperty("webdriver.chrome.driver", "./drivers/chromedriver.exe");

        WebDriver driver = new ChromeDriver();
        driver.get("https://"+username+":"+password+"@"+"the-internet.herokuapp.com/basic_auth");
        
        String text = driver.findElement(By.xpath("//*[@id=\"content\"]/div/p")).getText();
        String expected = "Congratulations! You must have the proper credentials.";
        org.testng.Assert.assertEquals(text.trim() , expected);
    }
}
 
