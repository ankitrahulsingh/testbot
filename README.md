# testbot
import selenium
from selenium import webdriver
from selenium.webdriver.common.action_chains import ActionChains
import time

driver= webdriver.Chrome()
driver.get("https://c6.avaamo.com/web_channels/444588bc-92fe-477f-87c1-88a92946346a/demo.html?theme=avm-messenger&banner=true&demo=true&banner_text=%20&banner_title=This%20is%20how%20the%20chat%20agent%20shows%20up")

time.sleep(10)

driver.find_element_by_xpath("//body/div[@id='avm_chat_widget_71bad76f-102c-465d-995a-d8e1f78b477c']/div[3]/a[1]/img[1]").click()

driver.find_element_by_xpath("//a[contains(text(),'Get Started')]").click()

driver.find_element_by_xpath("//body/main[1]/form[1]/div[1]/div[4]/div[1]/button[2]").click()




def msg():
    message=input("Enter your message")
    count=int(input("Enter the message count"))
    
    text_box= driver.find_element_by_xpath("//textarea[@id='queryTextbox']")
    
    for i in range(count):
        text_box.send_keys(message)
        driver.find_element_by_xpath("//button[contains(text(),'Send')]").click()
        
    msg()
    
    
    driver.find_element_by_xpath("//body[1]/main[1]/form[1]/div[1]/div[3]/button[1]").click()
    startover= driver.find_element_by_xpath("//a[contains(text(),'Start Over')]")
    
    startover.click()
    
    driver.find_element_by_xpath("//a[contains(text(),'Download Motor Policy')]").click()
    
    download=driver.find_element_by_xpath("//body[1]/main[1]/div[1]/div[1]/div[2]/section[1]/div[15]/div[1]/div[2]/div[1]/div[1]/div[1]/div[1]/div[2]/a[1]")
    
    download.click()
        
    
def msg():
    message=input("Test bot")
    name=driver.find_elements_by_xpath("//input[@id='popup-name']")
     
    text_box.send_keys(message)
     
    message=input("8789559096")
    contact=driver.find_element_by_xpath("//input[@id='popup-contact']")
     
    text_box.send_keys(message)
     
     
    action=ActionChains(driver)
    Home Insurance=action.move_to_element(Home Insurance).perform()
     
    driver.find_element_by_xpath("//body/div[3]/div[1]/div[1]/div[5]/div[1]/form[1]/div[3]/div[2]/div[1]/select[1]").click()
    
    submit= driver.find_element_by_xpath("//button[contains(text(),'Submit')]")
    
    submit.click()
    
    driver.find_element_by_id("utmcode").click()
    
    call=driver.find_element_by_xpath("//body/div[3]/div[1]/div[1]/div[6]/div[1]/div[1]/div[1]/img[1]").click()
    
    close=driver.find_element_by_xpath("//body/div[3]/div[1]/div[1]/div[5]/div[1]/form[1]/div[6]")
    close.click()
    
    driver.close()
