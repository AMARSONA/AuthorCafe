# AuthorCafe 

import org.openqa.selenium.By;
import org.openqa.selenium.chrome.ChromeDriver;

public class Login
{

	public static void main(String[] args) 
  {
		// TODO Auto-generated method stub
        System.setProperty("webdriver.chrome.driver", "C:\\Users\\win10\\Downloads\\browserdriver\\chromedriver.exe"); 
		ChromeDriver driver= new ChromeDriver();
         driver.get("https://authorcafe.com/sign-in/");
         driver.findElement(By.id("username")).sendKeys("aucsdet@yopmail.com");
         driver.findElement(By.id("signpassword")).sendKeys("Authorcafe@123");
         driver.findElement(By.className("signInSubmit signup-launch")).click();
           driver.findElement(By.className("emptyPaste")).sendKeys("Hello World");
         }
	

}
