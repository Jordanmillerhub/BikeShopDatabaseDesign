# BikeShopDatabaseDesign
Created an ER Diagram and converted it into a relationship schema for a Bike Shop
Entites were as followed:
● Employees have a store-issued ID number, a name, an address, and one phone
number.
● Customers have a store-issued ID number, a name, an address, and one or more
phone numbers. (this can be multi unlike employees.)
● The bike shop has numerous inventory items for sale at their store such as bikes,
accessories, clothing items, and other goods. Each inventory item is uniquely identified
by a SKU number (stock keeping unit). An inventory item also has a name, a type (i.e.
“bike”, “acc”, “clothes”), a description, a cost (i.e. the purchase cost for the bike shop), a
quantity, a Boolean-valued attribute called is_active that acts as a flag to indicate if the
product is currently active or not (this allows you to keep product/price history records).
Lastly, there is an attribute called reorder_level that is read by a trigger function and
possibly places a new record in a table called reorder if the quantity attribute value falls
below the reorder_level attribute value. 
*Note that a SKU number is unique to a product, so all of the black mountain bikes of a
particular make and model have some SKU number, and all the red mountain bikes of
the same make and model have a different SKU number.*
● The bike shop has numerous rental_bikes that are uniquely identified by a store-issued
ID number, a bike type (i.e. “road”, “mountain”, “bmx”), an hourly rental rate, and a
commission date that indicates when the bike was first commissioned as a rental.
● The bicycle shop maintains sales records for inventory items, also called sales_orders.
A sales_order record contains a unique store-issued transaction ID number, the date, the
subtotal, the tax, and the total sale cost. Similar to any shopping receipt, we must
maintain a list of inventory items sold in the transaction. We can not use a single
attribute to record what was bought, because we can purchase multiple items at a time.
