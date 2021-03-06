---
# This repository is for implementing a replica of google slides.

Following are the usecases.
Build a powerpoint (ppt) web application. You can refer Google slides for UI. The web application should support below use cases.

1) As a user, I should be able to see a white slide (white background) for adding text and image objects.

2) As a user, I should be able to see a toolbar with text and image icon.

3) As a user, I should be able to add a text object on the slide by clicking the text button.

4) As a user, I should be able to edit a text object by clicking it. When the text object is selected text formatting toolbar should be visible.

5) As a user, I should be able to apply bold, italics and underline on the text.

6) As a user, I should be able to add an image object on the slide by clicking the image button.

7) As a user, I should be able to able to resize both text and image objects by selecting the border of the object.

8) As a user, I should be able to drag and drop both text and image objects by selecting the border of the object.

Github Link: https://classroom.github.com/a/Ozv3pN3j

Guideline:

1) Follow git and coding best practices as the previous assignment.

2) You can only use text editor library. No other frameworks and libraries are allowed. You can use any text editor library for text formatting.


steps to use the application:
1. double click on slides.html file.
2.click on image/text button from the toolbar
3. on clicking the text button you will see a text box which is created in the canvas.
4.you can type your text in the textbox, as soon as you type you will see a toolbar to style your text as bold,italic,underline etc.
5. you can drag the textbox anywhere.
6. create multiple textboxes with text button in the toolbar
7.on clicking the image button, you will be given an option to browse the image in your computer, and once you select an image and click ok, image will appear
in canvas. you can drag the image anywhere
8. you can also resize the textboxes and images.

technical overview:
1. Entire fucntionality has been implemented using vanilla javascript and only CKEditor library for text formatting.
2. the eventlister is attached to text button, which takes care of creating the text box everytime the button is clicked, making the box draggable and resizable
3. The evernt listener is attached to image button, which checks if the selected file is an image by checking its format such as JPG,PNG etc, if it is an 
image the file gets uploaded and rendered using "readAsDataURL" method
4. Dragging and resizing takes place by identifying the current place of textboxes in the canvas, capturing top-left,top-right,bottom-left and bottom-right poition and manipulating 
it as needed.


References:
https://www.w3schools.com/howto/howto_js_draggable.asp
https://medium.com/the-z/making-a-resizable-div-in-js-is-not-easy-as-you-think-bda19a1bc53d
https://www.google.com/slides/about/
### Quick start

```bash
# clone the repo
git clone https://github.com/neu-mis-info6150-fall-2018/extra-credit-assignment-ppt-CharmyDesai306.git

# change directory to repo
cd example-app

# Use npm or yarn to install the dependencies:
npm install

# OR
yarn

# start the server
ng serve
```

N