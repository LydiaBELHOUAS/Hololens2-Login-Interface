# HoloLens 2 - Login Interface with REST API Integration

## 📝 Description
This project focuses on the development of a **login and account management interface** for the **Microsoft HoloLens 2**, integrating:
- A **front-end application** using **C#** and **XAML** for user interaction.
- A **back-end REST API** for user registration, authentication, and level management.

After login, users are redirected to Unity scenes (Level 1, Level 2, and Level 3), representing different tasks/games that collect and manage user data.

---

## 🚀 Features
1. **Login Interface**:
   - User authentication (username and password).
   - "Forgot Password" functionality.
2. **Account Management**:
   - User registration (with details like username, email, date of birth, etc.).
3. **REST API**:
   - User registration and login endpoints.
4. **Scene Management**:
   - Level-based navigation (Level 1, Level 2, and Level 3).
   - Data collection for user profiles.

---

## 🛠️ Tools and Technologies

### Front-End
- **C#** and **XAML**: For building the login interface.
- **Visual Studio 2019**: IDE for UWP (Universal Windows Platform) development.

### Back-End
- **.NET Core 6**: For building the REST API.
- **Newtonsoft.Json**: For handling JSON data serialization/deserialization.
- **Swagger/OpenAPI**: For API documentation.

### Mixed Reality Development
- **Unity 2020.3.x LTS**: Long-term support version compatible with HoloLens 2.
- **Mixed Reality Toolkit (MRTK) v2.8.3**: A toolkit for developing HoloLens 2 applications.
- **HoloLens 2 Emulator**: For testing the app without a physical device.

### Deployment
- **Device Portal**: To deploy UWP applications to HoloLens 2.
- **Visual Studio Build Tools**: For building and deploying UWP apps.

---

## 📦 Project Setup

### System Requirements
- **OS**: Windows 11 (64-bit).
- **Hardware**:
  - Processor: Intel Core i5 or higher.
  - Memory: 8 GB RAM minimum (16 GB recommended).
  - Storage: At least 20 GB of free space.
  - **HoloLens 2** device or emulator.

### Software Versions
- **Unity**: 2020.3.x LTS
- **Visual Studio**: 2019 (Community/Professional/Enterprise)
- **MRTK**: 2.8.3
- **.NET Core**: 6.0 or higher

---

## 🔧 Installation and Usage

### Clone the Repository
```bash
git clone https://github.com/LydiaBELHOUAS/Hololens2-Login-Interface.git
cd Hololens2-Login-Interface

Setting up the Front-End
Open the Hololens2-Login-Interface solution in Visual Studio 2019.
Select x86 or ARM64 as the target platform (depending on your HoloLens 2 setup).
Build and deploy the solution to your HoloLens 2 device or emulator.
Setting up the Back-End
Navigate to the API folder.
Open the API project in Visual Studio 2019.
Run the API locally or deploy it to a server (e.g., Azure or AWS).
Unity Scene Deployment
Open the Unity project in Unity 2020.3.x LTS.
Import MRTK v2.8.3.
Configure the project for UWP Build Settings:
Target SDK: Universal 10
Target Device: HoloLens
Architecture: x86 or ARM64
Build the project and deploy it via Device Portal.
🛠️ REST API Documentation
Endpoints
POST /register: Create a new user account.
Payload Example:

json
Copier le code
{
    "username": "john_doe",
    "email": "john.doe@example.com",
    "password": "SecurePassword123!"
}
POST /login: Authenticate an existing user.
Payload Example:

json
Copier le code
{
    "username": "john_doe",
    "password": "SecurePassword123!"
}
GET /profile: Retrieve user profile data.
Headers:

makefile
Copier le code
Authorization: Bearer <access_token>
For more details, refer to the swagger.json file included in the repository or open the Swagger UI in your browser.

📚 Resources and Documentation
Official Documentation
Microsoft HoloLens 2 Docs
Mixed Reality Toolkit (MRTK)
Unity Mixed Reality Toolkit
Tutorials and Guides
Getting Started with HoloLens 2
REST API Development with .NET Core
Unity UWP Build Guide
🛡️ License
This project is licensed under the MIT License.
You are free to use, modify, and distribute the code under this license.

👩‍💻 Author
Lydia Belhouas

GitHub: LydiaBELHOUAS
Email: lydiabelhouas5@gmail.com
