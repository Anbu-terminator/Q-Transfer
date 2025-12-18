Q-Transfer – Quantum Secure File Encryption & Decryption Platform

Q-Transfer is a secure file encryption and decryption system built using a FastAPI backend and a Vite + React frontend, with encrypted data stored in MongoDB.

Important: 

The backend must be running before using the frontend.


1.Live Deployment URLs:-

Backend (API Server):

->https://q-transfer-backend.onrender.com/

Frontend (User Interface):

->https://q-transfer-frontend.vercel.app/


2.Mandatory Execution Order:-

->First run the Backend, then use the Frontend

->The frontend depends entirely on the backend APIs for encryption and decryption.


2.1 Backend Setup & Running Instructions:-

->Navigate to Backend Root Folder
Make sure you are in the root directory where `requirements.txt` exists.

->Install Dependencies:

pip install -r requirements.txt

->Run the backend server:

uvicorn app.main:app --reload 

2.2Frontend Setup & Running:-

->Make sure you are in the root directory where package.json exists.

->Install Dependencies:

npm install

->Run the backend server:

npm run dev



Application Flow:-

Encryption Flow:

->User uploads a file via frontend

->User sets a password

->File is encrypted using quantum-entropy logic

->Encrypted file is stored in MongoDB

->A unique File ID is generated

Decryption Flow:

->User enters the File ID

->User enters the correct password

->File is decrypted on the backend

->Original file is downloaded securely

->Wrong password or File ID results in complete decryption failure.

Notes:-

->Always ensure the backend server is running before using the frontend.

->The frontend will not work independently.

->Encryption and decryption are handled only by the backend.

->MongoDB is used for encrypted file storage.

Technology Stack:-

->Backend: Python, FastAPI, Uvicorn

->Frontend: Vite, React, TypeScript

->Database: MongoDB

->Hosting: Render (Backend), Vercel (Frontend)

Status:

✔ Backend Deployed & Live
✔ Frontend Deployed & Live
✔ Encryption & Decryption Working
✔ Production Ready

Author: Q-Transfer Team
Project Type: Secure File Transfer & Encryption System
