# Put responsive on a website !
Responsive is a adjectiv of the term website wich informatically means that the website adapts its display to different screen widths.
## Introduction 
Hello everyone, thank you for checking my guide to put responsive into an html website ! When a website is responsive, it means that it creates dynamic changes to the appearance of the page, depending on the screen size and orientation of the device being used to view it. To visualize responsive, let's say that if i code that a kitten image into my page, it should appear only when the screen width is bigger than 500px : it means that most mobile users visiting my page won't see the kitten image but that somebody on a computer can. We can seet that responsive is very important for design measures and user experience, responsive is needd so that a website has a clear display on any device possible : it is frustrating if someone needs a computer to use properly your food-delivery If responsive is still not celar, making this project will make you understand or you can go through the "documentation" section to see for yourself. As i said, responsive is very important for me because i think that anyone visiting my website should not be using its brain or have dislay issues when visiting it, i think it should be the same for your website(s) too :) .
## Utilities
You need these things to make a responsive website, you can change some softwares depending on your personal preferences : 
- A software in which you can code HTML and CSS (version 5 and 3 at least), use [Visual Studio Code](https://code.visualstudio.com/) if you don't have any.
- A recent and updated version of an internet browser like google chrome or firefox
- Some space on your hard-drive
- A mouse (or mousepad), keyboard, hands and a brain :)
# The PASTA project
## Setting up our project
To start off, create a folder in which you will work on your project. In this folder, you will create another folder for CSS, fonts, image (in general we name it assets), inside create your CSS file (name it stlyles to avoid confusion), then make an html file which is your website (again, named generally index.html). You should have something like below : 

![Screenshot1](https://github.com/DeltaDave12/readme-project/blob/main/assets/Screenshot1.JPG)

Now we are ready to start coding our website !
## Making the PASTA website
Do not forget to tell the computer that your are in HTML and to link the HTML and CSS files ! Here is what I wrote for my website, try to keep the same structure and to make the same classes to understand the responsive part. The website is very simple because we want to demonstrate how to put responsive, not how to make a beautiful website. It's a simple recipe on how to make pasta !

Basic HTML structure :
```HTML
<!DOCTYPE html>
<html>
<head>
<title>Make a good pasta dish</title>
</head>
<body>
</body>
</html>
```

HTML Code :
```HTML
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8" />
    <title>Make a good pasta dish !</title>
    <link rel="icon" href="./assets/website-pasta-icon.png">
    <link rel="stylesheet" href="./assets/styles.css">
</head>
<body>
    <div>
        <div class="flex-h1">
            <p class="Head1">Dishes</p>
            <p class="Head1">Nutrients</p>
            <img class="small-image" alt="IconApps" src="https://cdn.iconscout.com/icon/free/png-256/apps-3114467-2598245.png">
            <p class="SignIn">Help</p>
        </div>
    </div>
    <div>
        <h2> Welcome to my website, i'm gonna show you how to make a delicious pasta dish !</h2>
    </div>
    <div>
        <img class="big-image" alt="Pasta1" src="./assets/pasta1.jpg" width="600px" height="300px">
    </div>
    <div>
        <h3>Origin</h3>
        <p>Carbonara is one of Rome's four classic pastas (cacio e pepe, amatriciana, and gricia are the others). There are a slew of theories about its possible origins, including:

            It was invented by Italian carbonari (charcoal workers) who prepared the dish on their shovels over a fire.
            The name refers to the ground black pepper in the dish that resembles flecks of coal (carbone means charcoal in Italian).
            It was a marrying of traditions between American soldiers in Italy during World War II and their bacon and egg rations with the local pasta dishes.</p>
    </div>
    <div>
        <h3>Ingredients</h3>
        <div>
            <p>Pasta</p>
        </div>
        <div>
            <p>Salt</p>
        </div>
        <div>
            <p>Eggs</p>
        </div>
        <div>
            <p>meta</p>
        </div>
    </div>
        <h3>How to make</h3>
        <p>
            Add bacon and water to a skillet and bring to a simmer
        </p>
        <p> Continue simmering until water is evaporated, then continue to cook the bacon until crispy.
        </p>
        <p> Remove bacon from pan and reserve the drippings.
                Saute garlic in that same skillet until golden brown, then add to a bowl with 1 tablespoon bacon fat, eggs, egg yolk, Parmesan and pepper. Mix well
        </p>
        <p>Meanwhile, cook the spaghetti or linguine pasta     until al dente. Once cooked, drain pasta and reserve 1 cup of the cooking water.
        Slowly pour the hot cooking water into the egg mixture. Then pour over the hot pasta and toss to coat. Add crumbled bacon.
        </p>
        <p>
        Let pasta rest for a few minutes, tossing frequently until the carbonara sauce thickens. Serve immediately with a sprinkle of fresh parsley.
        </p>
    </div>
</body>
</html>
```


CSS Code :
```CSS
html{
    background-color:rgb(102, 87, 199);
}


.flex-h1{
    display: flex;
    justify-content: flex-end;
    align-content: flex-start;
    align-items: center;
    gap: 15px
}

.small-image{
    width: 25px;
}

.big-image{
    width: 80%;
}
```

What the user sees on the Browser :

![Screenshot1](https://github.com/DeltaDave12/readme-project/blob/main/assets/Screenshot2.JPG)

## Put responsive into the PASTA project

To put responsive on our website, we must add media queries which is a coding technique to add responsivness to our website ! We are gonna put off the images of the website and center our elements when the page is lower than 600px.

Add CSS code for responsivness : 
```css
@media only screen and (max-width : 600px){

body {
    display : flex;
    flex-direction: column;
    align-items: center;
}

img{
    display: none;
}
}
```

The "@media" part is the one that puts responsivness. If you put it in your code, you will see the results as we previously wanted !

# Documentation
Download VS Code : https://code.visualstudio.com/download
Download Google Chrome : https://www.google.fr/chrome/?brand=CHBD&gclid=CjwKCAiAs92MBhAXEiwAXTi258cCpu4vCuVUoblktOwAQJc7k6bC-kp-dqB4qVlV4lkHI3YKap2_EBoC1WYQAvD_BwE&gclsrc=aw.ds
Info on media queries : https://www.w3schools.com/Css/css3_mediaqueries_ex.asp
General questions : https://stackoverflow.com/
More information about html and css : https://www.w3schools.com/html/default.asp
The code and ressources are in this directory !
# Conclusion

As you can see, putting responsivness isn't that hard but we've just touched the tip of the iceberg. Yes responsivness is when the page adapts to its width and height but fro some it's also when an element has a hoover or when some items work differtently with oder conditions. In all honesty, the bigger part will be to desingn a front and back-end with organisation for your website. Have a nice day and thank you for reading !
## A big thank you to...
nesrine toumi
EFREI Paris
StackOverflow and webmdocs
