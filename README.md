package pkg1;

import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class class1 {

	public static void main(String[] args) throws InterruptedException {
		// TODO Auto-generated method stub
        
		
		System.setProperty("webdriver.chrome.driver", "D:\\driver\\chromedriver.exe");
		
		WebDriver dr=new ChromeDriver();
		dr.get("https://www.amazon.in/?&ext_vrnc=hi&tag=googinhydr1-21&ref=pd_sl_28ors6rnjl_b&adgrpid=60611463244&hvpone=&hvptwo=&hvadid=294136260910&hvpos=&hvnetw=g&hvrand=15057160998030723723&hvqmt=b&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9050488&hvtargid=kwd-298319537966&hydadcr=15413_1904556&gclid=CjwKCAjwu_mSBhAYEiwA5BBmf9_nNE9Zu8y7PXCCSQtL7b7r70QYa0iY9ffJbGQZoNaALE4_p4GY0hoCjwQQAvD_BwE");
		
		
		Thread.sleep(2000);
		
		dr.navigate().to("https://www.flipkart.com/");
		//dr.close();//single tab close
		//dr.quit();//close all tab
		Thread.sleep(2000);
		
		dr.navigate().refresh();
		
		Thread.sleep(2000);
		
		dr.navigate().back();//back to Previous tab
		
		Thread.sleep(2000);
		
		dr.navigate().forward();//forward to nxt tab
		
		Thread.sleep(2000);
		
		dr.manage().window().maximize();
 	}

}
