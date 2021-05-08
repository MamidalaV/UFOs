# UFOs

## PURPOSE:
The purpose of this project is to create a web application usong HTML and JavaScript that has the data of all UFOs sighted in Unites States between Jan 1, 2010 and Jan 13, 2010. 

## RESULTS:

### Data Source: 
Data source provided for this project is a JavaScript file. The file can be found ![HERE](https://github.com/MamidalaV/UFOs/blob/main/static/js/data.js) and image of the same is included here as a sample.

![datafile](https://user-images.githubusercontent.com/74985818/117519416-5c526100-af71-11eb-877e-c4569f22a072.png)

### Webpage layout:
The layout has of the webpage is divided as below to fit all the essential requirements:

![layout](https://user-images.githubusercontent.com/74985818/117519772-0383c800-af73-11eb-9c02-148b9b339f2d.png)

### HTML Code:
- After setting up the bootstrap components, we linked the `index.html` file to the CSS file that is used to style the website.

![bootstrap_html](https://user-images.githubusercontent.com/74985818/117519970-fca98500-af73-11eb-8539-db2b31c468a9.png)

- In the body of the HTML file, a `navbar` has been included and hyperlinked to the the webpage itself. This way, the title in the navbar acts as a refresh button for the page.

![navbar](https://user-images.githubusercontent.com/74985818/117520126-bacd0e80-af74-11eb-9f25-fb85f77f0d56.png)

- Using **jumbotron**, the webpage is divided into various components to match the webpage layout mentioned above.

![design](https://user-images.githubusercontent.com/74985818/117520265-56f71580-af75-11eb-9e42-8c1a150ef57b.png)

- We then created an Unordered List (UL) that has multiple list items (li) where each listitem takes an input from the user.

![ul_list](https://user-images.githubusercontent.com/74985818/117520323-a89fa000-af75-11eb-9b2b-fa955545143f.png)

- A table is created with the following headers to match the data source.

![table_html](https://user-images.githubusercontent.com/74985818/117520349-c3721480-af75-11eb-853f-be6bf86b2f7b.png)

- Finally, we call the sources of the 'd3' library, JS files that has the underlying javacode for the application to run and importantly, the data file.

![sources](https://user-images.githubusercontent.com/74985818/117520356-ce2ca980-af75-11eb-9533-ffd12ff46915.png)

### Webapp using JavaScript:

The code for this application can be found ![HERE](https://github.com/MamidalaV/UFOs/blob/main/static/js/app.js). And the build of the application can be best described this way:
- **Step 1:** Bring in the data
- **Step 2:** Get table references using "tbody" tag.
- **Step 3:** Loop through each object in the data and append a row and cells for each value in the row of the table.
- **Step 4:** Loop through each field in the data row and add each value as a table cell.
- **Step 5:** Create a variable to keep track of all the filters as an object.
- **Step 6:** Create a function to update the filters variable.
- **Step 7:** Save the Id, Value and Element that was changed as a variable.
- **Step 8:** Using an IF condition, add the entered Id & Value to the filters list. Otherwise, clear that filter from the filters object.
- **Step 9:** Create another function to filter the table when data is entered.
- **Step 10:** Loop through all of the filters and keep any data that matches the filter values.
- **Step 11:** Rebuild the table using the filtered data
- **Step 12:** Finally, include a listener event for changes to each filter.

### Functionality:

- Upon launching the page, all records of data in the `data.js` file loads into the table within the webpage.
- Using the filters provided for Date, City, State, Country and Shape of the UFO, you can filter the data as needed.
- Once a value is entered into any of these input fields, the listener event added in the JavaScript will automatically pick up the value and filters the data.
- You can enter one of the 5 or all of the input values to slice the data as needed.

#### Example:
![filter_sample](https://user-images.githubusercontent.com/74985818/117520915-ee119c80-af78-11eb-8872-934dbea29a25.png)


## Summary:

