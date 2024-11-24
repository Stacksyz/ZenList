# ZenList

ZenList is a sleek and user-friendly Minecraft server list and status checker website.<br>
It allows users to add, browse, and monitor Minecraft servers while maintaining a clean and efficient design.

---

> [!CAUTION]
> You are **NOT** allowed to host this repository to the public!<br><br>
> THIS PROJECT IS LICENSED UNDER A CUSTOM LICENSE:
>
> * PERSONAL USE IS ALLOWED
> * PUBLIC HOSTING OR REDISTIBUTION OF THE CODE WITHOUT SUBSTANTIAL MODIFICATIONS IS PROHIBITED! SEE THE [LICENSE](./LICENSE) FILE FOR MORE DETAILS.
---
## Features

### General Features
- **Minecraft Server Listings**: Add your favorite servers to the list and explore other servers with detailed information.
- **Real-Time Status Checker**: View live server statuses, player counts, and other metrics.
- **User Accounts**: Log in with Discord to manage your servers and contributions. (more ways to log in will be available soon)

### User Features
- **Add Servers**: Submit your own Minecraft server with details such as the name, IP address, description, and more.
- **Manage Your Servers**: Edit or delete the servers you've added.
- **Server Approval System**: Submitted servers go through an admin approval process before being publicly listed.

### Admin Features
- **Admin Dashboard**: Approve, deny, edit, or delete server submissions.
- **User Moderation**: Manage user permissions and ensure fair use of the platform.

---

## Installation

> [!NOTE]
> Make sure you have the following installed:
> - [Node.js](https://nodejs.org/) (v16 or higher)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/stacksyz/zenlist.git
   cd zenlist
2. Install dependencies:
   ```bash
   npm install
3. Configure environmental variables:
   * Create a `.env`file in the root directory with the following values:
     ```makefile
     PORT=3000
     MONGO_URI=your_mongodb_connection_string
     SESSION_SECRET=your_session_secret
     DISCORD_CLIENT_ID=your_discord_client_id
     DISCORD_CLIENT_SECRET=your_discord_client_secret
     DISCORD_CALLBACK_URL=http://localhost:3000/auth/discord/callback
     ```
4. Start the development server:
   ```bash
   npm run dev

### File Structure
```bash
ZenList/
├── public/                # Static assets (CSS, JS, images)
│   ├── css/
│   ├── js/
│   └── images/
├── routes/                # Express route handlers
│   ├── authRoutes.js
│   ├── serverRoutes.js
│   └── adminRoutes.js
├── views/                 # EJS templates
│   ├── index.ejs
│   ├── login.ejs
│   ├── server-list.ejs
│   ├── add-server.ejs
│   └── admin-dashboard.ejs
├── models/                # Mongoose models
│   ├── Server.js
│   └── User.js
├── .env                   # Environment variables (not included in the repo)
├── app.js                 # Main application entry point
├── package.json           # Dependencies and scripts
└── README.md              # Project documentation
```
### Contribution
Contributions are welcome! To contribute:
1. Fork the repository
2. Create a new branch for your feature or bug fix:
      ```bash
      git checkout -b feature/your-feature-name
      ```
3. Commit your changes and push to your fork.
4. Open a pull request describing your changes.


### Contact
Have things you want to discuss regarding collaborations/projects etc. you can contact us at:

Discord: stacksyz <br>
Discord Server: [discord.gg/WvmNAEzuzg](https://discord.gg/WvmNAEzuzg) <br>
Email: [ZenDevelopment@gmail.com](mailto:zendevelopment@gmail.com)
