# React-Loopback-File-Storage
upload file to loopback Storage

cd loopback-api 
npm install 

cd myapp
npm install
#####################################
1. config root File
# loopback-api/server/datasources.json

"storage": {
    "name": "storage",
    "connector": "loopback-component-storage",
    "provider": "filesystem",
    "root": "./files"
  }

2. config client API
#myapp/src/App.js
axios.post('http://localhost:3000/api/attachments/assets/upload', data, {
