# Currency-converter-Website
In this Project (Currency Converter), I used HTML, CSS and JS to design a webpage which converts the currencies of five different countries and displays the result when you select the amount and the currency. 
Algorithm used:
Exchange Rates:
Exchange rates for converting from USD to other currencies are defined as constants (usdToEurRate, usdToGbpRate, usdToJpyRate, usdToInrRate).
Conversion Functions:
convertCurrency(): This function is called when the "Convert" button is clicked. It retrieves the user input (amount and source currency), converts the amount to USD using the convertToUSD function, and then displays the converted amounts in Euros (EUR), British Pounds (GBP), Japanese Yen (JPY), and Indian Rupees (INR) using the convertFromUSD function.
convertToUSD(amount, sourceCurrency, usdToEurRate, usdToGbpRate, usdToJpyRate, usdToInrRate): Converts an amount from the source currency to USD using switch statements based on the source currency.
convertFromUSD(amountInUSD, destCurrency, usdToDestRate): Converts an amount from USD to the destination currency using switch statements based on the destination currency.
HTML Elements:
Input elements include a text input for the amount (<input type="number" id="amount" ...>) and a dropdown for selecting the source currency (<select id="sourceCurrency" ...>).
The "Convert" button triggers the convertCurrency() function (<button type="button" onclick="convertCurrency()">Convert</button>).
The converted currencies are displayed in a <div> with the id "result" (<div class="result" id="result"></div>).
An image is displayed below the result (<img src="Image.jpg" alt="Image" width="70%">).
Styling:
External styling is applied through a CSS file (style.css) linked in the head of the HTML file.
Additional Notes:
The code utilizes basic error handling with throw new Error for cases where an invalid source or destination currency is provided.
The displayed result includes converted amounts for EUR, GBP, JPY, and INR.
The image with the alt text "Image" is displayed at the bottom of the page.

CSS Algorithm:
Resetting Default Styles:
The margin and padding for the elements (body, h1, h2, label, input, select, button, div) are set to 0 to reset some default browser styles.
Basic Styling for the Body:
The overall styling for the body includes setting the font family, background color, text color, line height, and additional padding. This provides a basic and consistent style for the entire page.
Styling for Header (h1):
The h1 element (presumably the main title) is styled with a specific text color, margin at the bottom, centered text alignment, and a larger font size.
Styling for Form Elements (label, input, select, button):
Labels are set to be block elements with a bottom margin.
Input, select, and button elements are given a consistent margin at the bottom, padding, and a width of 100%. The box-sizing property ensures that padding and border are included in the total width of the elements.
Custom Styling for Select Element:
The select element is styled to have a custom appearance. The default dropdown arrow is removed, and a background image (arrow.png) is added. This allows for a custom dropdown arrow icon.
Styling for the Convert Button:
The button element is styled with a background color, text color, and a pointer cursor. On hover, the background color changes to provide a visual indication.
Styling for Result Display (#result):
The element with the id "result" is styled with a top margin, bold font weight, and centered text alignment. This is likely the area where the converted currency results are displayed.
Additional Header Styles (h2):
Another header (h2) is styled with a specific text color, top and bottom margins, centered text alignment, and a larger font size.
Styling for the Image Container (.Image):
The .Image class is styled to use a grid layout with centered items. This is likely used for centering the image on the page.
Styling for Result Container (.result):
The .result class is styled with centered text alignment and a specific font size. This is likely used for styling the result display area.

