# Getting started with XERTE XOT Theme

The DigED XOT Theme provides great flexibility when it comes to customising the look and feel of your own project. Follow this guide to see how you can change some of the css properties to create a unique project of your own.

!!! note

    You don't need any prior knowledge of CSS but you should be comfortable with code.

## Changing the theme colour

Colours can be changed quite easily by altering the [custom properpties](https://developer.mozilla.org/en-US/docs/Web/CSS/--*) within the project.

To change the main theme colour:

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
   
3. Paste the code into the Styles field. This would allow you to overwrite the default css properties.
   ![styles field in project properties](https://i.imgur.com/hTUxuVP.png)

4. Choose a colour of your choice and make a note of the HSL value. In this example, I used [Google Colour Picker](https://g.co/kgs/m4765a) to pick a colour that I liked. Note down the hsl value `246, 90%, 33% `.

    !!! note

        Feel free to use any colour tools you like but make sure you note down the hsl value of the colour.

5. Go back to your Xerte project and apply the new values to the Styles

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

6. Click ` Play ` button to preview the changes. You should be able to see the new colour been applied to the title page as well as the header area.
   ![The title page with new colour](https://i.imgur.com/CiTLQEk.png)


## Updating the Title Page

1. Click on the Title Page and find the **Styles** field
2. Locate the following code:

    ```css
    /*pseudo element for gradient overlay, with fallback colour options*/
    #x_mainHolder::before {
        content: ' ';
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        opacity: 0.95;
        background: linear-gradient(105deg, var(--clr-accent) 55%, transparent 55%);
        background: radial-gradient(ellipse 75% 150% at bottom right, transparent 0%, transparent 75%, var(--clr-accent) 75%);
    }

    ```

3. Comment out the last line of code which gives the shade a rounded effect

    ```css

    #x_mainHolder::before {
        content: ' ';
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        opacity: 0.95;
        background: linear-gradient(105deg, var(--clr-accent) 55%, transparent 55%);
        /*background: radial-gradient(ellipse 75% 150% at bottom right, transparent 0%, transparent 75%, var(--clr-accent) 75%);*/
    }

    ```

4. You may also play with the ` background: linear-gradient(105deg, var(--clr-accent) 55%, transparent 55%); ` property to change the angle of the shade.
