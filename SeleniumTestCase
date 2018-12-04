package PHPTestCase;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;

public class PHPEval {
	public static void main(String[] args) {
		System.setProperty("webdriver.chrome.driver", "C:\\Users\\Shawn\\Desktop\\chromedriver_win32\\chromedriver.exe");
		
		// First Initialize the browser
		WebDriver driver = new ChromeDriver();
		/* driver.manage().timeouts().implicitlyWait(3, TimeUnit.SECONDS); */
		
		// Open PHP.net
		driver.get("http://www.php.net");
		
		// Maximize browser
		driver.manage().window().maximize();
		
		// Identify the textbox first before entering our text 'eval'
		WebElement Searchbox = driver.findElement(By.name("pattern"));
		
		// Now Enter the text 'eval'	
		Searchbox.sendKeys("eval");
		
		// And now enter/submit the text for search
		Searchbox.submit();
		
		// Check if we are on the correct page, match it with the correct exact Eval URL
		if(driver.getCurrentUrl().startsWith("http://php.net/manual/en/function.eval.php")) {
			System.out.println("Success, you are on the correct page.");
		}
		else {
			System.out.println("Failure, this is not the correct page. The Correct Page should be 'http://php.net/manual/en/function.eval.php'");
			//Assert.fail ("Test Failed, incorrect page");
			//return -1; // Fail Test
		}
		
		// Now Look for the word 'Caution'
		if (driver.getPageSource().contains("Caution")) {
			System.out.println("The Text 'Caution' was found.");
		}
		else {
			System.out.println("The Text was 'Caution' was not found.");
			//Assert.fail ("Test Failed. The text 'Caution' is not found");
			//return -1; // Fail Test
		}
	}	
}
