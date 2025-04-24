package seleniumlearn;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.support.ui.Select;
import org.testng.annotations.Test;
public class seleniumlearn {

	@Test
	public void myTest() {
		System.setProperty("webdriver.chrome.driver", "./drivers/chromedriver.exe");
		WebDriver driver = new ChromeDriver();
		driver.get("https://the-internet.herokuapp.com/dropdown");
		WebElement Dropdown = driver.findElement(By.id("dropdown"));
		Select sel = new Select(Dropdown);  
		sel.selectByVisibleText("Option 1");
		WebElement selected = sel.getFirstSelectedOption();
		System.out.println(selected.getText());
		
		
		}
}
