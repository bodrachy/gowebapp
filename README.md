**Project Overview:**
GO Web_App is a sample CRUD web application project implemented in Golang, utilizing HTTP, templates, OS, and SQL. It integrates Bootstrap 4, DataTables, MySQL, and Docker for seamless development and deployment.

**Getting Started:**
Follow these steps to set up and run the project on your local machine for development and testing purposes. Refer to deployment notes for live system deployment.

**Prerequisites:**
Ensure the following software is installed:
- Golang (preferably version 1.16)
- MySQL Database
- Docker (optional)

**Installation:**
1. Clone the repository:
   ```
   git clone https://github.com/le4ndro/gowt.git
   cd gowt
   ```
2. Install dependencies:
   ```
   go mod download
   ```
3. Create MySQL database and table (as specified in the code).

**Configuration:**
Create a .env file with the following variables and customize values:
```
DATABASE_NAME="gowtdb"
DATABASE_USERNAME="user"
DATABASE_PASSWORD="pass"
DATABASE_SERVER="localhost"
DATABASE_PORT="3306"
```

**Run Application:**
Execute the command:
```
make run
```

**Deployment:**
1. Build executable:
   ```
   make build
   ```
2. Run the application:
   ```
   ./out/bin/gowt
   ```
   (or `\out\bin\main.exe` on Windows)

**Docker Deployment:**
- Build and tag image locally:
  ```
  make docker-build
  ```
- Push image to registry:
  ```
  make docker-release
  ```
- Run Docker image locally:
  ```
  make docker-run
  ```

**Technologies Used:**
- Golang (programming language)
- Bootstrap 4 (HTML framework)
- jQuery (JavaScript library)
- DataTables (Advanced tables plug-in for jQuery)
