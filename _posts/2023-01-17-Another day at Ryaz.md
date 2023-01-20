## Another Day at Ryaz
Today, I am on course II of Code with Mosh - The Ultimate HTML5 & CSS3 Series. Part 2 in which I went through the topics of typography, Images, and Forms.
Here are the brief highlights of each of them

**1.Typography:** Text takes up to 80% of the whole website and it becomes pretty important to know about the usage of each property which makes up the text. There were many sub-topics that were discussed.

The first and foremost topic was **“styling fonts”**  where I got to know about web-safe fonts which can be accessed through any web browser. There are already built-in fonts in the VS code, which can be accessed through a shortcut:
**“font-family: (ctrl+space)”** There are various properties which are font-weight which discusses the boldness of the text, then we have font style which can be any italic, or any other style of your choice, up next is the font size, as the name suggests it describes the size, finally we have font-colour which is the color of the font.

Cool tip: in font color, if we have to provide the hex code and the first and last letters are same the we can use only the first three letters. For example: for #000000 is for black, we can use #000 which represents the same.

Then, studied the **Embedding web fonts,** which we can do with the help of many open-source. For example, MyFonts.com, google fonts, etc.
**Flash of Unstyled Text(FOUT)** was the most amazing part to learn about, there are some fonts that we embed from online websites but it takes some time to reload on the user’s browsers, so we already provide the web-safe fonts along with them, so that the user can experience the web-safe font until the online fonts get loaded, there are various properties under consideration in font-display: swap, fallback, block, optional.
Next, we have the **font stack** which has all the fonts which are supported by the different browsers.  In **vertical spacing,** we have two attributes to define, the first is Margin, which is the distance between the content and border and the other one is line height, which adjusts the vertical distance between the lines. The tip here is that whenever you ought to change the font size, it is necessary to change the line height. Discussing **Horizontal Spacing,** we have three attributes, the line-spacing which is the space between two lines, then we have word-spacing which is the space between the words. Lastly, it is width. It is always better to choose the absolute measure(px) rather than relative measures (rem). The ideal line length is 50 to 70 characters. In **Formatting Text,** we have various properties which we can modify in order to make it more attractive to read, namely, i)text-align, ii)text-indent, iii)text-decoration, iv)transform,v)white-space, vi)text-overflow, vii)column, viii)direction. 


**2. Images:** Images are another very crucial part of the websites, text is never enough to make the website look better. In this part of the course, I covered some sub-topics discussed below:
The first one was the **types and formats** of the image. There are two types of images first the raster image and second, the vector image. The raster image is a collection of pixels and these are captured by the camera the format is JPG, PNG, GIF, etc. whereas the vector image is mathematical for example Icons, Logos, etc. These are made up of the software and the format is SVG(scalable vector graphics). The image tag has two attributes to define the source(src) which is the file name and the alt which asks the user to provide descriptive text for the picture, then we have **CSS sprites**this is of great use to optimize the HTTP request. CSS sprite is grouping all the images together in a folder and then uses it directly in the CSS file, by doing this the HTML has to send only one request to the server rather than asking for much stuff. But there is a disadvantage first being that it will increase the size of the file and the second is that it is not flexible, if we want to add more images to the webpage, we need to make the sprites again. There is another way of optimizing the HTML request is by using **Data URLs***, for each image we can make a URL and embed it directly into the HTML file. But it has issues as well, for example, it increases the complexity and it is slow on mobile. **Clipping** is another feature that can be of utmost use to the developer. Sometimes we want to clip the images in certain shapes to make them look prettier, we have certain online software which makes our job easier, we can directly search CSS clip generators, and they give us the CSS code according to our preference. Then we have **Filters**, they are especially used when we have to show the special effects when we hover over a particular tab. This can be done using the code. 
```
“Img: hover{
filter: blur  (3px), grayscale(70%)”
}
```
If we want to search for more filters, search by CSS filter file. There are different types of screens that need different types of images, for the normal screen we want an image of 1x, for a bigger we might need an image of 2x. There are two types of resolutions one is the physical resolution which talks about the physical properties of the image and the logical resolution is how they behave, when we say 200px, we are referring to the logical resolution. The third most important concept is the **Device Pixel Ratio(DPR)** which is the ratio of physical resolution and logical resolution. High-density screens are those that have DPR>1. High-quality screens would have perfect images and are applied only to fixed-size images. Since different screens have different resolutions, to make it more efficient we use **Resolution Switching,** here we find out the responsive image breakpoints and set a condition in CSS that when this size is met, display the image of this size. Font icons are another special feature that adds spice to web pages, we can use fontawesome.com to download the fonts whose code can be embedded in the same. 


**3. Forms:** Forms play a crucial part to collect information, for the registration process and many other purposes. In this course, many changes which can be made to the forms are discussed below
The code to create a simple form is:
```
<form>
<label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```
In the input type, we type the format in which we are expecting our answer from the user. In the label, we specify the class of the response so that, we can be sure that the answer is to that question or label. We have various **frameworks** in the CSS, the most popular being Bootstrap, and then we have Foundation and milligram. Although Bootstrap is the most used but milligram is better and easier than bootstrap.  Then I went through the text fields, In text-field, a user has to enter the response with the help of a keyboard, we can limit the word count and also we have the place-holder option which is represented below:

 Then we have the data-lists,  we provide the user with the options to select from.the code for that is given below:
 ```
<datalist id=”Countries”>
<option value="India">
<option value="Canada">
<option value="America">
<option value=” United Kingdom">
<option value="Pakistan">
</datalist>
```
Up next were the **drop-down lists**, as the name suggests which also provide options, the difference is that we use a select tag rather than datalist. Then we can style the forms according to our choice we can have checkboxes(more than one option is selected) and radio buttons(only one option is selected) as per our preferences.
```
<form>
    <ul style="list-style-type:none;">
      <li><input type="checkbox" name="language" value="HTML" />HTML</li>
      <li><input type="checkbox" name="language" value="CSS" />CSS</li>
      <li><input type="checkbox" name="language" value="JavaScript" />JavaScriptt</li>
    </ul>
   </form>
 ```
Then we have **Sliders,** which are used when we have more text on our page but we provide the users with the slider rather than increasing the size of the container or decreasing the font size. In forms, we can also provide the user with the option of submitting files called file inputs, in order to design it to our preferences we make the necessary changes we can allow the user to upload only the files with a certain format or the number of files accepted. Moreover, we can group the related fields with the help of the <fieldset> tag. Sometimes, we have the answers to some questions which are supposed to pop up after the submission and are meant to be hidden from the user called **“hidden fields”** then they will be stored in the server but won’t be able to show up to the user. Data is the real currency and redundancy in data calls for data preprocessing which deletes the meaningless answers, so it is always better to do the data validation for example if we are asking the user to enter the email, does that contain @ symbol if not then the server will not accept that answer, it reduces the chances of adding meaningless stuff as the answer to the question. The last step in the forms is “Submitting the form”, we have two METHODS (how the user sends the response) first is the GET where the fields don’t get added to the body of HTML instead get appended in the target URL and the second one is the POST, where the fields(responses) get added to the HTML requests. To get the response we fill in the “action” tab with the absolute URL. Another way, we can create an online form using formspree.io where you can create a form and get the link to embed it in the HTML file and then the responses can be checked from the website only. 

This was all for the day!!
  
Quite a long day but fruitful!
  
See you in the next blog!





 
	
