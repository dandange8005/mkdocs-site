# Getting started with XERTE XOT Theme

The DigED XOT Theme provides great flexibility when it comes to customising the look and feel for your own project. Once you've installed the theme, you can 

## Change the colour

The theme uses css [custom properties](https://developer.mozilla.org/en-US/docs/Web/CSS/--*) to control variety of things including colours, font-family etc.

Below is the default custom properites in the theme:

```css title="default custom properties"

:where(html) {


    /*Title page*/
    --clr-accent: hsl(217, 59%, 20%);
    --clr-h: 217;
    --clr-s: 59%;
    --clr-l: 20%;

    --gradient-image: url('https://images.unsplash.com/photo-1614850523459-c2f4c699c52e?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2850&q=80');


    /*Header background colour*/
    --clr-header-bg: var(--clr-accent);

    /*Footer background colour*/
    --clr-footer-bg: #495057;

    /*body colours*/
    --clr-body-bg: var(--shade-sand); // body background
    --clr-body-text: var(--neutral-8); // main body text colour
    --clr-headline: var(--black); //headline colours
}



```