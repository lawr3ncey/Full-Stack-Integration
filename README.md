# InventoryHub – Full Stack Inventory Management App

**Project Owner:** Lawrence Babelonia

InventoryHub is a full-stack inventory management system built with **Blazor WebAssembly** (front-end), **.NET Minimal API** (back-end), and integrated with **Microsoft Copilot** for AI-assisted development.

---

## Features

- View a product list with name, price, stock, and category
- JSON-based data exchange between client and server
- Nested object structure: Product includes a Category
- Optimized API with in-memory caching (`IMemoryCache`)
- CORS-enabled secure API access
- AI-assisted development via GitHub Copilot

---

## Tech Stack

- **Front-end:** Blazor WebAssembly
- **Back-end:** .NET 9.0 Minimal API
- **Data:** In-memory mock data + caching
- **Security:** CORS policies applied

---

## Getting Started

### Prerequisites

- [.NET SDK 9.0](https://dotnet.microsoft.com/download)

### Run ServerApp

```bash
cd ServerApp
dotnet run
```

The API will run on `http://localhost:5000`

### Run ClientApp

```bash
cd ClientApp
dotnet run
```

The Blazor app will run on `http://localhost:5001`

---

## API Endpoints

### GET /api/productlist

Returns a list of products with nested category objects.

**Response Example:**
```json
[
  {
    "Id": 1,
    "Name": "Laptop",
    "Price": 1200.50,
    "Stock": 25,
    "Category": {
      "Id": 101,
      "Name": "Electronics"
    }
  }
]
```

---

## Project Structure

```
InventoryHub/
├── ClientApp/          # Blazor WebAssembly frontend
│   ├── Pages/
│   │   └── FetchProducts.razor
│   └── Program.cs
└── ServerApp/          # .NET Minimal API backend
    └── Program.cs
```

---

## Key Implementation Details

### Caching Strategy
The backend implements `IMemoryCache` with a 5-minute TTL to optimize performance and reduce redundant data processing.

### CORS Configuration
CORS is configured to allow cross-origin requests between the Blazor client and the API server.

### Data Models
- **Product**: Contains Id, Name, Price, Stock, and a nested Category object
- **Category**: Contains Id and Name

---

## Development with Microsoft Copilot

This project was developed with AI assistance from GitHub Copilot. See [REFLECTION.md](REFLECTION.md) for insights on the AI-assisted development process.

---

## License

This project is for educational purposes.

---

## Author

**Lawrence Babelonia**
