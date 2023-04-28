# Getting started with XERTE XOT Theme

The DigED XOT Theme provides great flexibility when it comes to customising the look and feel of your own project. Follow this guide to see how you can change some of the css properties to create a unique project of your own.

!!! note

    You don't need any prior knowledge of CSS but you should be comfortable with code.

## Changing the theme colour

Colours can be changed quite easily by altering the [custom properpties](https://developer.mozilla.org/en-US/docs/Web/CSS/--*) within the project.

To change the main theme colour,

1. Copy the code below

    ```css title="default custom properties"
    :where(html) {
        /*Accent colour*/
        /*Main accent colour controls the title page shade and the page header background */
        --clr-accent: hsl(217, 59%, 20%);
        --clr-h: 217;
        --clr-s: 59%;
        --clr-l: 20%;
    }
    ```
2. Open you XOT project
   
3. Paste the code into the Styles field
   ![styles field in project properties](https://i.imgur.com/hTUxuVP.png)

4. Choose a colour of your choice. 
   
   !!! note

        Feel free to use any colour tools you like but make sure you note down the hsl value of the colour.


   In this example, I used [Colour Picker](https://g.co/kgs/m4765a) to pick a colour that I liked. Note down the hsl value `246, 90%, 33% `, change the value next to each property 
   ```css title="Example"
    :where(html) {
    /*Accent colour*/
    /*Main accent colour controls the title page shade and the page header background */
    --clr-accent: hsl(246, 90%, 33%);
    --clr-h: 246;
    --clr-s: 90%;
    --clr-l: 33%;
    }
    ```