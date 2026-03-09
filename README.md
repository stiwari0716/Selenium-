# Selenium-
Navigation Commands:  

import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class NavigationExample {

    public static void main(String[] args) {

        WebDriver driver = new ChromeDriver();

        driver.get("https://example.com");

        driver.navigate().to("https://google.com");
        driver.navigate().back();
        driver.navigate().forward();
        driver.navigate().refresh();

        String currentUrl = driver.getCurrentUrl();
        String title = driver.getTitle();

        System.out.println("Current URL: " + currentUrl);
        System.out.println("Title: " + title);

        driver.quit();
    }
}
