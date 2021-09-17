# The Validation Process
## CSS
No errors were found when running the style.css file through the test on jigsaw.w3.org.  
![Test result css](assets/images/readme_images/no_error_css.png)

## HTML
All html pages were run through validator.w3.org.
### index.html
The first attempt of validating the index.html file gave these errors:  
![Index file errors](assets/images/readme_images/error_index.png)  
- Error number 2 through 4 was caused by an easy mistake. I had forgotten to add id:s to the input fields of the change schedule form.
When those were added, the errors were solved.  
![Index file errors fix](assets/images/readme_images/error_index_fix.png)  
  
- Error number 1 was not obvious to me how to solve since I didn't have a database where to send the information or a thank you page where I could send the user. But this issue got solved by adding the javascripts, which closes the form and opens the thank you note, to the action.  
![Index file error fix](assets/images/readme_images/error_index_fix_2.png)

### about-us.html
The first attempt of validating the about-us.html file gave this error:  
![About-us file error](assets/images/readme_images/error_about.png)
- I had missed a semicolon after the pound sign. It was easily fixed.  
![About-us file error fix](assets/images/readme_images/error_about_fix.png)

### apply-here.html
The first attempt of validating the apply-here.html file gave these errors:  
![Apply-here file error](assets/images/readme_images/error_apply.png)  
- Error number 4 and 5 was caused by me missing the id on input fields, again. The errors were fixed by just adding those.  
![Apply-here file error fix](assets/images/readme_images/error_apply_fix.png)  

- Error number 1 through 3 took some iteration before it was solved.
  - First I focused on the tip "The first option element ... must have either an empty value attribute, or must have no text content" and tried to enter an extra empty option first.  
  ![Apply-here file error fix](assets/images/readme_images/error_apply_fix_2.png)  
  But this only resulted in yet another, not very clear, error:  
  ![Apply-here file error](assets/images/readme_images/error_apply_2.png)
  - Then I tried to approach the error with "Consider adding a size attribute..."  
  ![Apply-here file error fix](assets/images/readme_images/error_apply_fix_3.png)  
  This worked as far as solving the error, but it gave an input field that didn't look very good in the browser.  
  ![Apply form with size attribute](assets/images/readme_images/apply_form_w_size_attr.png)
  - Ok, what do I do? I had to google "consider adding a placeholder option label" and found this page: [w3docs.com](https://www.w3docs.com/snippets/css/how-to-create-a-placeholder-for-an-html5-select-box-by-using-only-html-and-css.html)  
  With this help I tried adding placeholders on each select option.  
  ![Apply-here file error fix](assets/images/readme_images/error_apply_fix_4.png)  
  Finally the errors were solved and the form looked good.  
  ![Apply form with placeholder option](assets/images/readme_images/apply_form_w_placeholder.png)  

### thank-you.html
No errors were found when running the thank-you.html file through the test on validator.w3.org.

## Lighthouse check
I was pretty happy with the lighthouse check on desktop:  
![Lighthouse check on desktop](assets/images/readme_images/lighthouse_desktop.png) 

The first lighthouse check on the mobile device was not as good:  
![Lighthouse check on mobile](assets/images/readme_images/lighthouse_mobile.png)  
But after changing the size of the hero image, and compressing it again,  
![Compressing hero image](assets/images/readme_images/comp_hero_img.png)  
the result was much better:  
![Lighthouse check on mobile](assets/images/readme_images/lighthouse_mobile_2.png)

## Notepad++
I used Notepad++ to check the code for missing quotes. There I found one class and one id where I had missed the quotes:  
![Check in Notepad ++](assets/images/readme_images/check_notepad.png)  