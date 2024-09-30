 erDiagram
   %% Defining the entities and relationships for the Nike Shoe Store
    products {
        string name
        string size
        string model 
        string size
        string price
        string gender
    }
  Customer {
         int CustomerID
         string First name 
         string last name
         string email ID
         string phone number
         string address 
    }
  Order { 
         order number
         order delivery 
    }
  Sales {
         int SaleID
         int ProductID
         int CustomerID
         int Quantity
         string Paymentmethod
    }
  Inventory {
          int InventoryID
          int ProductID
          int StockeAdd
          Date Restokdate
    }
  %% Rrelationships {
         Customers ||--o{ Sales : makes
         Products ||--o{ Sales : sold_in
         Products ||--o{ Inventory : restocked_in
         
