# ASPCoreWebAPICRUD 🧠

A simple ASP.NET Core Web API project demonstrating full CRUD operations with JWT-based authentication.

## 🚀 Features

- ✅ CRUD operations for **Student** entity (Create, Read, Update, Delete)
- 🔐 JWT Authentication & Token generation
- 🔐 Authorization-protected endpoints
- 🧪 Swagger UI for testing API endpoints
- 🛠️ Entity Framework Core with SQL Server LocalDB

---

## 🗂️ Tech Stack

- ASP.NET Core 7/8
- Entity Framework Core
- SQL Server LocalDB
- JWT Bearer Authentication
- Swagger (Swashbuckle)

---

## 📁 Folder Structure

ASPCoreWebAPICRUD/
│
├── Controllers/ # API Controllers (StudentController, AuthController)
├── Models/ # Model classes (StudentModel, UserModel)
├── Services/ # JWT Token generation service
├── Data/ # DbContext and configuration
├── appsettings.json # App configuration & JWT settings
├── Program.cs # Application startup
└── ASPCoreWebAPICRUD.csproj


---

## 🔧 Setup Instructions

### 1. Clone the Repo

```bash
git clone https://github.com/your-username/ASPCoreWebAPICRUD.git
cd ASPCor

2. Update Appsettings

"Jwt": {
  "Key": "thisIsMySuperSecureKey@1234567890", // must be at least 256 bits (32 chars)
  "Issuer": "ASPCoreWebAPICRUD"
}
3. Run the Application

dotnet restore
dotnet run
Navigate to: https://localhost:7014/swagger

🔐 Test Authentication
1. Login
POST /api/Auth/login

json
Copy
Edit
{
  "username": "admin",
  "password": "admin123"
}
🔁 Response: JWT token

2. Use the Token
Click Authorize button on Swagger UI and paste the token:

Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...

Now you can access protected routes.

📬 Contact

For questions or contributions, feel free to open an issue or pull request.

IMGS:

<img width="1920" height="1080" alt="Screenshot 2025-07-28 165510" src="https://github.com/user-attachments/assets/6822cd46-591b-4ee6-845b-1906fdd7e151" />
<img width="1829" height="706" alt="Screenshot 2025-07-28 172035" src="https://github.com/user-attachments/assets/e7f99cbd-9f59-44e9-b74d-81f5df324479" />



