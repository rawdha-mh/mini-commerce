# 🛒 Mini Commerce

This is a full-stack Laravel e-commerce mini platform running in a Docker environment using **Laravel Sail**. It’s designed as a practice project to learn Laravel, Docker, authentication (Breeze), and MySQL integration.

---

## 🚀 Features

- Laravel 12 (via Laravel Sail)
- MySQL, Redis (Sail default stack)
- Laravel Breeze – authentication scaffolding
- Dockerized environment with `docker-compose`
- Blade + AlpineJS frontend
- Vite for asset building

---

## 📦 Project Structure

mini-commerce/
├── backend/ # Laravel app
│ ├── app/
│ ├── bootstrap/
│ ├── config/
│ ├── database/
│ ├── public/
│ ├── resources/
│ ├── routes/
│ ├── storage/
│ └── ...
└── README.md # This file


---

## 🛠️ Installation & Setup

### Prerequisites

- [Docker Desktop](https://www.docker.com/products/docker-desktop)
- [WSL2](https://learn.microsoft.com/en-us/windows/wsl/) (if on Windows)

### 1. Clone the repository

git clone https://github.com/rawdha-mh/mini-commerce.git
cd mini-commerce/backend

### 2. Start Laravel Sail

./vendor/bin/sail up -d

### 3. Install frontend dependencies

./vendor/bin/sail npm install
./vendor/bin/sail npm run dev

## ⚙️ Configuration
 
### 1. Rename .env.example to .env if not already done:

cp .env.example .env

### 2. Generate app key: 

./vendor/bin/sail artisan key:generate

### 3. Set custom APP_URL and DB_PORT if needed.

## 🧪 Migrate Database

./vendor/bin/sail artisan migrate

## 📝 Roadmap

Product catalog

Shopping cart

Checkout flow

Admin dashboard

Testing (PHPUnit)

## 🤝 Contributing

Contributions are welcome! Feel free to fork and submit pull requests.

## 📄 License 

MIT


