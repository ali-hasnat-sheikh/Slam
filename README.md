# ⚡ Slam — Searchable Log of All Messages

> **Slam** ("Searchable Log of All Messages") is a modern, real-time Slack clone engineered with a decoupled architecture for instant messaging and reliable data persistence.

---

## 🏗️ Architecture & Features

* **"Two-Brain" Design:** Decouples heavy CRUD operations (REST API) from instant message delivery (WebSockets).
* **Workspace & Channel Sharding:** Multi-tenant architecture supporting private channels and isolated workspaces.
* **Instant RTM (Real-Time Messaging):** Live message broadcasts, real-time typing indicators (`user is typing...`), and active presence tracking.
* **Searchable Message Log:** Organized message history stored persistently in PostgreSQL, ready for fast indexing and querying.
* **Authentication:** Seamless and secure token-based login via Google OAuth.

---

## 🛠️ Tech Stack

| Layer | Technology |
| :--- | :--- |
| **Backend API** | Python (FastAPI), Uvicorn |
| **Database & ORM** | PostgreSQL (Supabase), SQLAlchemy |
| **Real-Time Engine** | Native FastAPI WebSockets / Connection Managers |
| **Authentication** | Google OAuth 2.0 / Custom JWTs |