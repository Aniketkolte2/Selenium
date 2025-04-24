package seleniumlearn;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.annotations.Test;
public class seleniumlearn {

	@Test
	public void myTest() {
		System.setProperty("webdriver.chrome.driver", "./drivers/chromedriver.exe");
		WebDriver driver = new ChromeDriver();
		driver.get("https://the-internet.herokuapp.com/login");
		String title = driver.getTitle();
		System.out.println(title);
		WebElement name = driver.findElement(By.id("username"));
		name.sendKeys("tomsmith");
		WebElement pass = driver.findElement(By.id("password"));
		pass.sendKeys("SuperSecretPassword!");
		driver.findElement(By.xpath("//*[@id=\"login\"]/button")).click();
		driver.quit();
		}
}
