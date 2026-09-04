# StockFlow


## Architecture Diagram


                    ┌──────────────┐
                    │    React     │
                    └──────┬───────┘
                           │
                           ▼
                    ┌──────────────┐
                    │   Keycloak   │
                    │     IAM      │
                    └──────┬───────┘
                           │
                           ▼
                         JWT
                           │
                           ▼
                    ┌──────────────┐
                    │ YARP Gateway │
                    └──────┬───────┘
                           │
             ┌─────────────┼─────────────┐
             ▼             ▼             ▼
        Product API   Inventory API   Purchase API
          .NET 10         Go           .NET 10
             │             │             │
             ▼             ▼             ▼
        ProductDb     InventoryDb    PurchaseDb

        
