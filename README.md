# AIM:
To scrape product data from the Amazon shopping website and save it into a CSV file using UiPath.

# Software Required:
```
1.UiPath Studio
2.Web browser with UiPath extension (Chrome/Edge)
3.Active internet connection
```

# Procedure:
```
1.Create a new process in UiPath Studio.
2.Add a Use Browser activity:
   Set URL to:  "https://www.amazon.in/s?k=watches" (or any desired keyword)
3.Inside the Do section:
   a.Add a Table Extraction activity.
   b.Click on two similar product names to auto-detect the pattern.
   c.Select the fields like  product name,price and no of reviews per product, etc.
   d.Save the extracted data to a variable, e.g., ExtractDataTable.
4.After extraction, add a Write CSV activity
    Set ExtractDataTable as the input.
    Set output file path to something like: "C:\Users\YourName\Documents\WEBSCRAPING.csv"
    Enable Include Headers checkbox.
5.(Optional) Add a Message Box after writing to CSV to confirm success.
6.Run the workflow and wait for completion.
```

# Workflow:
![Screenshot 2025-05-08 140335](https://github.com/user-attachments/assets/39d9392a-8426-431d-805a-41ed2f2d6cd4)

# Output:
![Screenshot 2025-05-08 140435](https://github.com/user-attachments/assets/24a11cf1-8521-4fad-b8c3-92acdd75e03f)
![Screenshot 2025-05-08 140459](https://github.com/user-attachments/assets/fdfd498e-3a54-4b7b-ae00-e317c75272d8)



# Result:
Amazon product data is successfully extracted and saved in CSV format at the specified location and Web Scraping Process is successfully executed.



