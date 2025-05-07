package seleniumlearn;

import java.util.ArrayList;
import java.util.List;
import java.util.Set;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.annotations.Test;

import com.sun.org.apache.xerces.internal.impl.xpath.XPath;

public class seleniumlearn {

    @Test
    public void myTest() {
        System.setProperty("webdriver.chrome.driver", "./drivers/chromedriver.exe");

        WebDriver driver = new ChromeDriver();
        driver.get("https://demo.automationtesting.in/Frames.html");
        driver.switchTo().frame("SingleFrame");      
        driver.findElement(By.xpath("/html/body/section/div/div/div/input")).sendKeys("prasadchutiya");
        
        
    }
}
