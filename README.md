# My-Weather-Dashboard-Web-Application
API - Weather Dashboard
1. HTML
1) Creating a simple html skeleton - adding English as an language (lang="en"); translating machine code into human-readable text and vice versa to be displayed in the browser (<meta charset="utf-8">); controlling dimensions and scaling (<meta name="viewport" content="width=device-width, initial-scale=1.0">); telling Microsoft Internet Explorer users to use the latest rendering engine (<meta http-equiv="X-UA-Compatible" content="ie=edge" />)
2) Linking an empty (for now) css file - style.css
3) Creating a title - Weather Dashboard
4) Accroding the ss which was provided, we need to create a header that will be centered, with white text - according to the Bootstrap documantion:
- Creating the container-fluid class - provides a full width container, spanning the entire width of the viewport
- Padding utilities setting up to 2 
- Setting the background colour to dark - .bg-dark
5) Adding H1 - Weather Dashboard 
6) Setting up max and width resolutions by creating a div class
7) Creating a div class - row 
8) Creating a new class - left - to create a form (grid) : for a large screen, adding a padding-bottom - 3 
9) Creating a h2 element - Search for a City by using an id : margin top 1
10) Creating an Id and class for a form - using bootstrap documentation: 
- form-inline class to display a series of labels, form controls, and buttons on a single horizontal row
- form-group provides a flexible class that encourages proper grouping of labels, controls, optional help text, and form validation messaging. 
- input group to add text, buttons, or button groups on either side of textual inputs, custom selects, and custom file inputs. - In this case : "text","search-input","San Diego","form-heading", "today forecast"
- Adding a bootstrap class: .input-group-append
- Adding a search button 
11) Using Aria - https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Live_Regions
12) Using day.js to format dates
13) Adding js file 

2. CSS
- Set up the line height for all browsers - line-height
- Make sure that the font size will not adjust in iOS - When an element containing text uses 100% of the screen's width, the algorithm increases its text size, but without modifying the layout. The text-size-adjust property allows web authors to disable or modify this behavior, as web pages designed with small screens in mind do not need it.
Sections styling:
- Setting up up margin to 0 (all browsers)
- For a main element - Displays an element as a block element. It starts on a new line, and takes up the whole width - using display block 
- Setting up a font size and margin for H1 element (section and article) for different browsers 
- For the grouping elements we are adding the box size and hight 
- Adding an overflow property - Default. The overflow is not clipped. The content renders outside the element's box (what happens to content that is too big to fit into an area.)
- Using a pre tag - Preformatted Text element - text will be presented exactly as written in the HTML file. - using Monospaced font; and font size - 1em is equal to the current font size. The default text size in browsers is 16px. So, the default size of 1em is 16px.
Semantic styling:
- Setting up the background color of an element - transparent - Specifies that the background color should be transparent. This is default (to remove the gray background color)
- <abbr>: The Abbreviation element (https://developer.mozilla.org/en-US/docs/Web/HTML/Element/abbr) - to remove the bottom border, The text-decoration property specifies the decoration added to text 
- Adding the font weight - https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight
- <code>	Defines a piece of computer code
-  <kbd> tag is used to define keyboard input. 
- <samp>	Defines sample output from a computer program
Setting up the font and size 
- Adding the font size for the all browsers - small
- <sup> tag defines superscript text.
- <sub> HTML element specifies inline text which should be displayed as subscript for solely typographical reasons.
- Preventing from affecting the line height (all browsers)
- Removing a border on an imges
- On the forms - changing the font style, setting up a margin to 0
- Making sure that overflow is showing
- The text-transform property controls the capitalization of text - No capitalization. The text renders as it is. This is default
- Style clickable typy - The element is drawn like a button
- Removing the inner border and padding 
- Restoring the focus styles - -moz-focusring
- Setting up a correct padding 
- Correcting the text wrapping, color, removing the padding 
-  Adding the correct vertical alignment - https://developer.mozilla.org/en-US/docs/Web/CSS/vertical-align
- Removing the default vertical scrollbar
- Setting up the correct box size and removing the padding 
- Cursor style - https://developer.mozilla.org/en-US/docs/Web/CSS/::-webkit-inner-spin-button
- Adding outline style 
- Removing the inner padding
- Styling the clickable types and changing font properties to inherit
- Adding the correct display property 
- Creating height and width utilities styles 
- Adding margins on all sides 
- Adding margin bottoms 
- Adding margin tops 
- Adding margin - right
- Adding margin - left 
- Adding margin - x axis
- Adding margin - y axis
- Adding padding on all sides
- Adding padding bottoms 
- Adding padding tops 
- Adding padding - right
- Adding padding - left 
- Adding padding - x axis
- Adding padding - y axis
- Setting up styles for background utilities 
- Setting up styles for display properties 
- Setting up flex content properties 
- Setting up the style to make sure ut works with small, medium, large and extra large devices 

3. JS
- Setting up global variables : API key, API URL and Search History 
- Referencing all the DOM elements (document.querySelector)
- Adding timezone plugs - dayjs.extend
- Using a function to display the previous search - renderSearchHistory
- Runing a for loop to show the most recent search at the top
- When you click on the city from your search history (list on the left) it should show the informaion on hte main screen (data-search)
- Creating a function to update the search history in local storage and display 
- If nothing is in search - return the function 
- In order to get search history from the local storage we need to run a function - initSearchHistory
- To display the current weatehr we need to run the function to display the data from the API - renderCurrentWeather(city, weather, timezone)
- Creating vars to store the data 
- Running a function to display forecast card (from weatehr API) - renderForecastCard
- Setting up vars for the data that comes from api 
- Card - we need to create all the elements 
- Adding all the content to the elements - °F, MPH, % etc 
- Creating a function to display forecast for 5 days 
- Creating unix timestamps for start and end of the forecast 
- Runing a for loop - timezone
- Creating a function (fetchWeather) - to get the weatehr data for the given specific location, then we are calling this function to display the data 
- Adding another function if location is not added
- Returning the function if there is nothing in the search box 
- Returning the function if the element is not showing under search history 
- 



