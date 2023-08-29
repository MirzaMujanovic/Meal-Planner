### **🍽️ Intro**
The Weekly Meal Planner by A.M. is a powerful tool designed to help you effortlessly create a weekly meal schedule. Whether you're planning meals for yourself, your family, or an event, this tool streamlines the process and ensures that your meals are diverse and tailored to your preferences. Below, we'll guide you through how to use this tool and highlight its benefits.

#### **🛠️ Set Up the Environment**
   - Ensure you have R & RStudio installed on your computer
   - Save the R Notebook provided as "index.Rmd."
   - Install and load the necessary R packages: `tidyr`, `tidyverse`, and `googlesheets4`. You can do this using the `install.packages()` and `library()` functions in R.

#### **🌐 Authenticate with Google Sheets**
   - The tool utilizes Google Sheets as a data source. To access your Google Sheets, you'll need to authenticate your Google account with R. Use the `gs4_auth()` function, replacing `"YOUR_EMAIL@gmail.com"` with your Gmail address. This step grants the tool access to your Google Sheets.

#### **🍲 Prepare Your Meals in Google Sheets:**
   - Create a Google Sheet (or use an existing one) to list your favorite meals. You can access this sheet using this [link](https://docs.google.com/spreadsheets/d/13uEbDKVbkLz9PpYwXzOLZAgw_ZWppBm7pjnDbHnH9yA/edit#gid=0), and make a copy for yourself.
   - In the Google Sheet, include columns for "Meal_Name," "Type," "Prep_Time_min," "Recipe_Link," and "Effort." Fill in the details for each meal.

#### **💾 Export Google Sheet as CSV (Optional):**
   - You can export your Google Sheet as a CSV file if needed. However, this step is optional, as the tool can directly access Google Sheets.

#### **📊 Access Google Sheet Data:**
   - In the R Notebook, specify the URL of your Google Sheet using the `sheet_url` variable. Replace `"YOUR_GOOGLE_SHEET_URL"` with the actual URL of your Google Sheet.
   - Use the `googlesheets4::read_sheet()` function to load your Google Sheet data into R. The tool will automatically convert the data into a data frame for further processing.

#### **📅 Generate Your Meal Schedule:**
   - The tool generates a weekly meal schedule with three meals a day (breakfast, lunch, and dinner) for each day of the week (Monday to Sunday).
   - It ensures that meals are randomized and don't repeat within the same week.
   - The output provides details such as the meal name, preparation time, recipe link, and effort level.

### **🏆 Benefits**

**⏱️ Time-Saving.** This tool significantly reduces the time and effort required to create a weekly meal plan. Instead of manually organizing meals, the tool does it in seconds.

**🍽️ Diverse Meals.** By randomizing your meals, it helps ensure that you enjoy a variety of dishes throughout the week, preventing meal monotony.

**🔧 Customization.** You have full control over your meal choices. You can easily update your Google Sheet with new recipes or preferred meals, and the tool will adapt accordingly.

**🚀 Efficiency.** The tool is designed to be efficient and user-friendly. With just a few simple steps, you can generate a detailed meal plan tailored to your preferences.

**🌍 Access Anywhere.** Since your meal data is stored in a Google Sheet, you can access and edit it from anywhere, making meal planning a breeze even when you're on the go.
