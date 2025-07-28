## 🗳 NextGen Ballot – A Secure Digital Voting Platform
### NextGen Ballot is a modern, full-stack, secure and responsive digital voting web application built for hackathons and real-world scalability. It allows users to register, verify via Aadhaar & OTP (mocked), vote securely, and enables administrators to track total and remaining votes live.


## Features:

- Aadhaar and Voter ID-based authentication
- CAPTCHA + OTP verification
- Admin Dashboard with live results
- Secure voting with one-vote-per-user logic
- MongoDB integration for persistent storage
- Responsive and intuitive UI



## 🔧 How To Setup Things

### 1. 📦 Install Dependencies
Run the following command in your terminal:
```bash
npm install
```

### 2. MongoDB connection in .env file:

   ```bash
   MONGO_URI=mongodb+srv://<username>:<password>@cluster01.clagshx.mongodb.net/?retryWrites=true&w=majority&appName=Cluster01
   PORT=5000
   NODE_ENV=development
   ```
   Replace username and password with your MongoDB Atlas credentials.


### 3. Enable Network Access in MongoDB Atlas

After creating your cluster and getting your connection string, follow these steps:

1. Go to your MongoDB Atlas **Dashboard**.
2. Navigate to **Network Access** under the **Security** section in the left sidebar.
3. Click on **"Add IP Address"**.
4. Select **"Allow Access from Anywhere"** (adds `0.0.0.0/0`).

 > 🔒 For development only.

5. Click **Confirm**.

 > ⚠️ Without this step, your backend won't be able to connect to your MongoDB cluster.



### 4. Backend (Node Server):
Run the following command in your terminal:
```bash
node server.js
```

### 5. Dummy Data For Testing:

- Aadhar: 485663215457,   phone: 4523658795,   voter id: YJK7896554 
- Aadhar: 987465632445,   phone: 4654653157,   Voter id: RWT1236548
   
   Note: OTP will be logged in your terminal, not sent via SMS in this mock version.

### 6. Admin Login:

- Username: admin
- Password: admin123
