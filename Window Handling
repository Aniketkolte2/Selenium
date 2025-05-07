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
        driver.get("https://www.hyrtutorials.com/p/window-handles-practice.html");

        String parentWindow = driver.getWindowHandle();
        String titlehome = driver.getTitle();
        System.out.println("Parent window title: "+titlehome);

        driver.findElement(By.id("newWindowBtn")).click();

        Set<String> windowHandles = driver.getWindowHandles();
        List<String> windows = new ArrayList<String>(windowHandles);

        // Switch to the new window
        driver.switchTo().window(windows.get(1));

        String title = driver.getTitle();
        System.out.println("Child Window Title: " + title);

        // Optional: Close the child and switch back to parent
        
        driver.switchTo().window(windows.get(0));
        driver.findElement(By.xpath("//*[@id=\"newTabBtn\"]")).click();

        
    }
}

