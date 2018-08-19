# 100 Days Of Code - Log
### Day 13: August 18, 2018 Saturday

**Today's Progress**: MyFabricStashApp
Ok, so, I know that I've been MIA for awhile from the 100 days of code challenge, and I'm not going to make any excuses. I just didn't keep up with it. I'm trying not to look behind and move forward. I did get quite a bit accomplished today on MyFabricStashApp.  
* **HTTP 403 Forbidden Error on Receipts/Index** -- For some odd reason, HTTP was adding on a trailing slash at the end of the URL http://localhost:53163/Receipts/ instead of, http://localhost:53163/Receipts so it was doing a 301 Redirect Permanent. I simply created a new route in RouteConfig.cs and changed the URL to Receipt instead and it works fine for all CRUD views. 
* **Add ReceiptNumber to Model and Views** -- The controller now auto-generates the ReceiptNumber and stores it with the Receipt in the database. The Receipts List (Index) displays the Receipt Number in a column in the table.
* **Add Sources DropDownList to Receipts/Create view** -- The Dropdown list on Receipts/Create View gets list of sources from db and when form is submitted, sends id value of source to POST.
* **Source Name displays in Receipt List** -- The Source Name, i.e. "Joann" now displays in the Receipts List table, instead of the SourceID

**Thoughts:** Got a LOT accomplished today. Feeling pretty good about it, but there is still a lot more todo. 

**Link to work:** [MyFabricStashApp](https://github.com/khambley/MyFabricStashApp)

### Day 3: August 8, 2018 Wednesday

**Today's Progress**: FreeCodeCamp.org
Today I took a little break and worked on FreeCodeCamp, I'm trying to learn Javascript better, it never really was my strong suit, but Michael Jordan was a not so good free throw shooter and he practiced and practiced every day sometimes shooting 300 free throws a day! Now he is the all time free throw shooter! So that's my strategy for getting to be a pro at Javascript. 

**Thoughts:** I also had my final paper due in my Software Design class, so I did code as much as wanted to today. But, I get a 5-day break from classes, I'll spend that on coding.

**Link to work:** [FreeCodeCamp](https://freeCodeCamp.org)

### Day 2: August 7, 2018 Tuesday

**Today's Progress**: MyFabricStashApp(.NET MVC5, EF6, C#)
-Created a listing of Purchases for each Fabric on Fabric Details page. Learned about eager/lazy loading related queries using the "virtual" keyword

-Created a link on Fabrics Detail page for creating a new Purchase for an existing fabric. Created Dropdownlist for Receipts and Sources.

-Ran into a bit of a problem trying to pass the URL parameter, FabricId, to the Create page, inside the TextBox for fabricId. I wanted it to prepopulate the field when page loads. I googled it, stackoverflow, etc and finally came upon a simple solution. Put the FabricId in the Viewbag in the Controller, then use a TextBoxFor helper and retrieve the value from the ViewBag.  
In Create view, ```@Html.TextBoxFor(model => model.FabricId, new { @Value = ViewBag.FabricId })```  
It worked! I need to style it up a bit, figure out a way to add back html attributes but at least it is functioning.

**Thoughts:** I didn't work on this feature today so I'll keep it in here for my work tomorrow -> "I'd like to add the Fabric image swatch to the dropdownlist helper, but it is not going to be as simple as I thought. I found a couple tutorials on how to do it and I'll work on that tomorrow for the challenge. [ImagesInDropDownLists Tutorial](http://fairwaytech.com/2012/08/adding-images-select-lists-mvc3/)"

**Link to work:** [MyFabricStashApp](https://github.com/khambley/MyFabricStashApp)

### Day 1: August 6, 2018

**Today's Progress**: Continued work on an app I started back in February that stores and displays all the fabrics in my collection. It's called MyFabricStashApp. I'm working with the .NET MVC5 framework, and Entity Framework 6 migrations. 

-I'm working on the full list of requirements on my Github repo page.

-Added the Purchases List page and added to nav. 

-Added PurchasesListViewModel for the Purchases List

-DropdownList helper on Create view that lists all Fabrics to choose from. 

**Thoughts:** I'd like to add the Fabric image swatch to the dropdownlist helper, but it is not going to be as simple as I thought. I found a couple tutorials on how to do it and I'll work on that tomorrow for the challenge. [ImagesInDropDownLists Tutorial](http://fairwaytech.com/2012/08/adding-images-select-lists-mvc3/)

**Link to work:** [MyFabricStashApp](https://github.com/khambley/MyFabricStashApp)


