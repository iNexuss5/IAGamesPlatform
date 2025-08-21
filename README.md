[![Unity](https://img.shields.io/badge/Unity-2022.3.20f1-blue.svg)](https://unity.com/)
[![Azure](https://img.shields.io/badge/Deployed%20on-Azure-informational.svg)](https://azure.microsoft.com/)

## Contributors

[![Ana Carriço](https://img.shields.io/badge/Contributor-Ana_Carriço-pink)](https://www.linkedin.com/in/ana-carri%C3%A7o-b890ba296/)

# AI Games Platform (July 30, 2025)

This project focuses on implementing a gaming platform where users can compete both against other human players and against artificial intelligence systems.
The official documentation/report are written in portuguese. 

## How to Test?

The project was deployed using Microsoft Azure services, namely **WebApp** and **Flexible Server MySQL**.  
The `.php` files (containing UnityWebGL for game visualization) and the database were uploaded via FTP (FileZilla).  
This way, any user can test the platform without needing to install Unity.

It is available at:  
[AI Games Platform](https://notenoughgames-e8dke0edddhkckfc.spaincentral-01.azurewebsites.net) *(30-07-2025)*  

⚠️ A certificate may be required (automatic SSL certificates demand a private → paid domain).

### Cache Issues
The application has known caching issues, which may prevent some information from being properly updated. To fix this, we suggest:

- Reload the page with **Ctrl+F5**  
- Disable the site cache  

### Error Handling
No error-handling system has been implemented for unfinished games.  
Please make sure to finish all games to avoid malfunction.

---

## How to Recreate the Environment?

1. Install **Unity 2022.3.20f1** → [unityhub://2022.3.20f1/61c2feb0970d](unityhub://2022.3.20f1/61c2feb0970d)  
2. Create a **2D Project**  
3. Go to **Import Package > Custom Package** and select the file located in `\03_Implementation\Export`

---

## Project Structure

The directory `\03_Implementation\Code` is divided into three categories:

- **Unity C# Code** (`\Games`) → organized based on each script’s function  
- **PHP Code** (`\PHPs`) → manages the graphical interface (HTML + CSS + JS), Unity communication, and database connection  
- **Database Export** (`\DB`) → `.sql` dump of the database
