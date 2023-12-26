# Ex-07-CSS
Name:PREM.R

Reference Number: 23002486

Department: AIML

# Ex-07(i)-css

# AIM:

(i) Using CSS media queries, modify the webpage's color scheme with the following requirements:

#Default Color Scheme:

Background color: Light gray (#f4f4f4) Text color: Dark gray (#333) Link color: Blue (#007bff)

#Small Screen Adaptation (Max-width: 600px):

Change the background color to dark gray (#333) Change the text color to light gray (#f4f4f4) Change the link color to light green (#28a745)

#Dark Mode Preference:

If the user has set their device to dark mode, override the above styles with the following:

Background color: Black (#000) Text color: White (#fff) Link color: Cyan (#17a2b8)

#Deliverable:

Write the CSS code that implements the above requirements. Your code should include the base styles and the appropriate media queries for small screens and dark mode preference.

# DESIGN PROCEDURE:

# STEP 1:

Define the document type as HTML.

# STEP 2:

Open the HTML structure with the necessary head and body sections. In the head section, set the title of the webpage and define the styles for the webpage. The styles include: -->Default color scheme for the webpage. -->Adaptations for small screen sizes. -->Adaptations for users who prefer a dark color scheme.

# STEP 3:

In the body section, create a division with the text "Amazing places to visit". Also in the body section, create a list with links to the Discovery World, Christmas in Switzerand, Wonder la.

# STEP 4:

Close the HTML Structure.

# CODE:
```
<!DOCTYPE html>
<html>
    <head>
        <title>Media queries Ex:1(i)</title>
        <style>
            /Default Color Scheme/
            body{
                background-color: #f4f4f4;
                color: #333;

            }
            a{
                color: #007bff;
            }
            /Small Screen Adaptation/
            @media (max-width: 600px) {
                body{
                    background-color: #333;
                    color:#f4f4f4;
                }
                a{
                    color:#28a745;
                }
            }
                /Dark Mode Preference/
                @media (prefers-color-scheme: dark) {
                    body{
                        background-color: #000;
                        color: #fff;
                    }
                    a{
                        color: #17a2b8;
                    }
                }

        </style>
    </head>
    <body>
        <div>
            <h1>prem web page welcomes you</h1>
            <ul>
                <li><a href=https://chat.openai.com>Chatgpt welcomes you</a></li>
                <li><a href=https://www.wikipedia.org>wikipedia</a></li>
                <li><a href=https://www.youtube.com>youtube</a></li>
            </ul>
        </div>
    </body>
</html>
```
## OUTPUT :

#(i)Default-screen
![media queries 1](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/cf5b2c0d-79ae-4a89-be40-00c03af6cd18)


#(i)Small-screen adaptation
![MEDIA QUERIES 2](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/8da34f8e-fcab-4b68-a7b3-be49f9f4f362)

#(i)dark-mode
![MEDIA 3](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/c9b120f9-0736-430c-8321-58317d1590c2)


# Ex-07(ii)-css

# AIM:

To use a media query in CSS to apply different styles to a webpage for mobile devices (with widths less than 600px) and desktop devices (with widths greater than or equal to 600px)? Provide an example CSS snippet to demonstrate your answer.

# DESIGN PROCEDURE:

# STEP 1:

Start the HTML document and create the root element.

# STEP 2:

Inside , create the element and include a style element for CSS rules.

# STEP 3:

Define CSS rules for desktop devices. Use a media query to define CSS rules for mobile devices.

# STEP 4:

Create the element inside , which will contain the webpage content.

# STEP 5:

Inside , create a for the heading and an for the list of hyperlinks.

# STEP 6:

End the HTML document by closing all open tags.

# CODE:
```
<!DOCTYPE html>
<html>
    <head>
        <title>Media queries Ex:1(ii)</title>
        <style type="text/css">
            /CSS rules for desktop devices/
            body{
                background-color: blanchedalmond;
            }
            /CSS rules for mobile devices/
            @media only screen and (max-width: 600px){
                body{
                    background-color: plum;
                }
            }
        </style>
    </head>
    <body>
        <div>
            <h1>prem web page welcomes you</h1>
            <ul>
                <li><a href=https://chat.openai.com>Chatgpt welcomes you</a></li>
                <li><a href=https://www.wikipedia.org>wikipedia</a></li>
                <li><a href=https://www.youtube.com>youtube</a></li>
            </ul>
        </div>
    </body>
</html>
```
# OUTPUT:

#(ii)Desktop view
![media queries 7 b](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/a7236f09-0ea1-4152-a427-b63009618ad2)

#(ii)Mobile view
![media queries 7b 2](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/fc926441-6e02-4de8-9174-69a461b999e7)


# Ex-07(iii)-css orientation-based media query

# AIM:

To explain how you can use CSS media queries to apply different styles based on the orientation (landscape or portrait) of the device.Provide a CSS example where you change the background color of the body based on the orientation.

# DESIGN PROCEDURE:

# STEP 1:

Identify the section in your HTML file where you want to add the CSS. This is typically within the style tags in the section.

# STEP 2:

Define a CSS media query for each orientation. The syntax for a media query is @media (orientation: value), where value can be either portrait or landscape.

# STEP 3:

Within each media query, specify the CSS rules you want to apply. In this case, you want to change the background color of the body.

# STEP 4:

Close the media query with a }.

# STEP 5:

Repeat steps 2-4 for the other orientation.

# STEP 6:

Save your HTML file. Open your HTML file in a web browser and change the orientation of your device to see the different styles applied.

# CODE:
```
<html>
    <head>
        <title>Media queries Ex:1(iii)</title>
        <style type="text/css">
            @media (orientation: portrait) {
                body{
                    background-color: rgb(228, 236, 192);
                }
            }
            @media (orientation: landscape) {
                body{
                    background-color: rgb(235, 144, 238);
                }
            }      
            </style>
    </head>
    <body>
        <div>
            <h1>prem web page welcomes you</h1>
            <ul>
                <li><a href=https://chat.openai.com>Chatgpt welcomes you</a></li>
                <li><a href=https://www.wikipedia.org>wikipedia</a></li>
                <li><a href=https://www.youtube.com>youtube</a></li>
            </ul>
        </div>
    </body>
</html>
```
# OUTPUT:

#(iii)Landscape mode
![media queries 7c 1](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/198f4f15-e152-4acd-a0e4-106815fd6a98)

#(iii)Portrait mode 
![media queries 7c 2](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/f4d980cd-39ce-4773-a9a9-961f43e0b388)


# Ex-07(iv)-css responsive typography

# AIM:

To use media queries to adjust typography (like font size and line spacing) on a website to improve readability across different device sizes, from mobile phones to large desktop monitors. Include a CSS code snippet in your explanation.

# DESIGN PROCEDURE:

# STEP 1:

Identify the HTML elements you want to style. In your case, it’s the h1 and li elements.

# STEP 2:

Define the base styles for these elements. This will be the default styling that applies when no media queries match.

# STEP 3:

Use media queries to apply different styles for different device sizes. The @media rule is used in CSS to apply styles for specific media types/devices.

# STEP 4:

Inside the media queries, specify the device size for which the styles should apply. You can use min-width and max-width properties to target devices with widths within a certain range.

# STEP 5:

Adjust Typography: Inside each media query block, adjust the typography (like font size and line spacing) for the identified elements.

# STEP 6:

Test your styles.

# CODE:
```
<!DOCTYPE html>
<html>
    <head>
        <title>Media queries Ex:1(iv)</title>
        <style type="text/css">
            h1,li{
                font-size: 16px;
                line-height:1.5;
            }
            @media screen and (min-width: 600px){
                h1,li{
                    font-size: 18px;
                    line-height:1.6;
                }
            }
            @media screen and (min-width: 900px){
                h1,li{
                    font-size: 20px;
                    line-height: 1.7;
                }
            }
            @media screen and (min-width: 1200px){
                h1,li{
                    font-size: 22px;
                    line-height: 1.8;
                }
            }
        </style>
    <body>
        <div>
            <!DOCTYPE html>
            <html>
                <head>
                    <title>Media queries Ex:1(iv)</title>
                    <style type="text/css">
                        h1,li{
                            font-size: 16px;
                            line-height:1.5;
                        }
                        @media screen and (min-width: 600px){
                            h1,li{
                                font-size: 18px;
                                line-height:1.6;
                            }
                        }
                        @media screen and (min-width: 900px){
                            h1,li{
                                font-size: 20px;
                                line-height: 1.7;
                            }
                        }
                        @media screen and (min-width: 1200px){
                            h1,li{
                                font-size: 22px;
                                line-height: 1.8;
                            }
                        }
                    </style>
                </head>
                <body>
                    <div>
                        <h1>Amazing places to visit</h1>
                        <ul>
                            <li><a href=https://discoveryworld.org>Discovery World</a></li>
                            <li><a href=https://www.myswitzerland.com/en-in/experiences/winter/christmas>Christmas in Switzerland</a></li>
                            <li><a href=https://www.wonderla.com>Wonder la</a></li>
                        </ul>
                    </div>
                </body>
            </html>
```
# OUTPUT:

#(iv)600px
![7d 1](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/ce05a78e-c2ef-4664-822b-791c301eb1fd)

#(iv)900px
![7d  2](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/67f9bcfd-c3cc-40e6-a196-813044839f62)

#(iv)1200px 
![7d 3](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/914fdd13-e52d-4707-ad11-7bd5f191b760)


# Ex-07(v)-print-friendly css

# AIM:

To use a media query to change the styling of a webpage when it is printed, such as changing the background to white and hiding non-essential elements. Provide a CSS example.

# DESIGN PROCEDURE:

# STEP 1:

Identify the HTML elements you want to style. In your case, it’s the h1 and li elements.

# Step 2:

Define the base styles for these elements. This will be the default styling that applies when no media queries match.

# Step 3:

Use media queries to apply different styles for different media types. The @media rule is used in CSS to apply styles for specific media types/devices.

# Step 4:

Inside the media queries, specify the media type for which the styles should apply. You can use print to target printers.

# Step 5:

Adjust Styles: Inside each media query block, adjust the styles for the identified elements. You can change the background to white and hide non-essential elements.

# Step 6:

Test your styles using the print preview feature in browsers to ensure they work as expected.

# Step 7:

Iterate: Adjust your media queries and styles as needed based on your tests.

# CODE:
```
<!DOCTYPE html>
<html>
    <head>
        <title>Media queries Ex:1(v)</title>
        <style type="text/css">
            h1,li{
                font-size: 16px;
                line-height: 1.5;
            }
            @media print{
                body{
                    background-color: white;
                }
                h1,li{
                    font-size: 12px;
                    line-height: 1.4;
                }
                /Add any non-essential elements you want to hide when printing/
                .non-essential{
                    display: none;
                }
            }
        </style>
    </head>
    <body>
        <div>
            <h1>prem web page welcomes you</h1>
            <ul>
                <li><a href=https://chat.openai.com>Chatgpt welcomes you</a></li>
                <li><a href=https://www.wikipedia.org>wikipedia</a></li>
                <li><a href=https://www.youtube.com>youtube</a></li>
            </ul>
        </div>
    </body>
</html>
```
# OUTPUT:

#(v)Default page
![7e 1](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/bc70309c-5257-4e29-ab6d-b3150b879fcf)

#(v)Display none
![7 e 2](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/58b71745-8866-45f3-834c-40bb11928d91)

# Ex-07(vi)-Dark mode implementation

# AIM:

With the increasing popularity of dark mode in user interfaces, explain how you would use a media query to detect if the user has set their system to prefer a dark color scheme. Provide an example of how you would change the background and text colors of a website based on this preference.

# DESIGN PROCEDURE:

# Step 1:

Use the prefers-color-scheme media feature, which is used to detect if the user has requested the system use a light or dark color theme.

# Step 2:

The prefers-color-scheme media feature can have the values light, dark, or no-preference.

# Step 3:

In your CSS, you can use this feature within a @media rule to apply different styles depending on the user’s preference.

# Step 4:

You can set the background color to black and the text color to white when the user prefers a dark color scheme.

# Step 5:

Conversely, you can set the background color to white and the text color to black when the user prefers a light color scheme.

# Step 6:

If the user has no preference, you can choose a default color scheme.

# Step 7:

Remember to test your website in both light and dark modes to ensure the colors work well in both settings.

# CODE:
```
<!DOCTYPE html>
<html>
    <head>
        <title>Media queries Ex:1(vi)</title>
        <style type="text/css">
            body{
                background-color: white;
                color: black;
            }
            @media (prefers-color-scheme: dark){
                body{
                    background-color: black;
                    color: white;
                }
                a{
                    color: bisque;
                }
            }
            @media (prefers-color-scheme: light){
                body{
                    background-color: white;
                    color: black;
                }
            }
        </style>
    </head>
    <body>
        <div>
           <h1>Amazing places to visit</h1>
            <ul>
                <li><a href=https://chat.openai.com>Chatgpt welcomes you</a></li>
                <li><a href=https://www.wikipedia.org>wikipedia</a></li>
                <li><a href=https://www.youtube.com>youtube</a></li>
            </ul>
        </div>
    </body>
</html>
```
# OUTPUT:
![7f](https://github.com/PREM3112/ODD2023-WT-Ex-07-CSS/assets/145449383/7ad03455-17da-441d-9a83-92350d0acdfd)

# RESULT:
thus the output got successfully.
