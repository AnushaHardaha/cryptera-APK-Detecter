# 🛡️ Cryptera APK Security Scanner 🚀

Cryptera is an **advanced APK security scanner** designed to detect fake banking applications and analyze Android APK files for malicious behavior. The system provides comprehensive security analysis including **permission analysis, threat intelligence, and machine learning-based detection**.

---

## 🌟 Features

- **📦 APK Analysis**: Deep analysis of Android APK files including manifest parsing, certificate extraction, and DEX file analysis  
- **🏦 Banking App Detection**: Specialized detection for fake banking applications using pattern matching and behavioral analysis  
- **🔍 Security Scanning**: Comprehensive security analysis including permission analysis, string analysis, and obfuscation detection  
- **🛠️ Threat Intelligence**: Integration with VirusTotal and MalwareBazaar for real-time threat intelligence  
- **🤖 Machine Learning Detection**: AI-powered malware detection capabilities  
- **🖥️ RESTful API**: Easy-to-use REST API for programmatic access  
- **🌐 Web Interface**: User-friendly web interface for manual APK uploads and analysis  

---

## 💻 Technology Stack

- **Backend**: Node.js, Express.js  
- **Database**: MongoDB (optional)  
- **Security**: Helmet, CORS, Rate Limiting  
- **File Processing**: Multer, yauzl, xml2js  
- **Threat Intelligence**: VirusTotal API, MalwareBazaar API  
- **Logging**: Winston  
- **Frontend**: HTML5, CSS3, JavaScript  

---

## ⚙️ Prerequisites

- Node.js (version 16.0.0 or higher)  
- npm (Node Package Manager)  
- Optional: MongoDB for storing scan results  
- Optional: Android SDK Build Tools for advanced APK parsing  

---

## 📥 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/gourichouksey/cybershield.git
   cd cybershield
   ```

2. **Install dependencies**

    ```bash
   
         npm install
     ```
3. **Configure environment variables**
       ```bash

       cp .env .example .env
    ```
5. **Create required directories**

    ```bash

        mkdir -p uploads logs data
     ```

# 🛠️ Configuration

**Environment Variables**

- Copy .env.example to .env and configure the following variables:

- VIRUSTOTAL_API_KEY 🔑: Your VirusTotal API key (optional but recommended)

- MALWAREBAZAAR_API_KEY 🔑: Your MalwareBazaar API key (optional but recommended)

- ABUSEIPDB_API_KEY 🔑: Your AbuseIPDB API key (optional)

- PORT 🌐: Server port (default: 3000)

- NODE_ENV ⚙️: Environment (development/production)

**API Keys Setup**

1. VirusTotal API Key

- Visit VirusTotal

- Create an account and get your API key

- Add it to your .env file

2. MalwareBazaar API Key

- Visit abuse.ch Authentication Portal

- Create an account and get your API key

- Add it to your .env file

  # 🚀 Running the Server
  
**Development Mode**
      
  ```bash 
              
 npm run dev
   ```
**Production Mode**
       
  ```bash
               
               npm start
   ```
**Using PM2 (Recommended for Production)**
     
  ```bash 

            npm install -g pm2
            pm2 start server.js --name cybershield
            pm2 startup
            pm2 save
 ```
