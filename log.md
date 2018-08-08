# 100 Days Of Code - Log
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


