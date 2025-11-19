# HeritageGraph

HeritageGraph is an initiative taken by researchers at **CAIR-Nepal**.

While many individuals and organizations are doing remarkable work to preserve cultural heritage at the ground level, the growing trend is that today most users discover and interact with knowledge through the internet via browsers, search engines, and even chatbots like ChatGPT.

To make heritage truly accessible in the digital age, we need to go beyond physical preservation and digitally preserve, publish, and democratize access of knowledge where,

- 🕸️ **Crawlers** can crawl,
- 🤖 **Agents** can interact,
- 👩‍💻 **Developers** can query, and
- 💬 **Users** can seek answers through chatbots.

We intend to provide **unparalleled digital access** to the knowledge of our shared heritage.

---

## 🌏 Why Cultural Heritage?

There is a powerful quote:

> _“If you want to know where we should head in the future, then you should know where we came from our past, our shared understanding of it, and the experiences of our forefathers. These things serve as a strong moral compass for where to go and what to pursue in the future.”_

Heritage is not just memory, it’s **direction**.

---

## 🚀 Getting Started

Sounds interesting and want to try it out?

Clone the repository:

```bash
git clone https://github.com/CAIRNepal/CHLOD
```

Switch to the working branch (`v1`):

```bash
git switch v1
```

### Quick Test with Docker

If you just want to test and see the current progress:

```bash
docker compose up --build
```

---

If you want to contribute :-) \
Here is a guide for setting up frontend and backend.

## 🖥️ Frontend

The frontend is built with **Next.js** and uses **shadcn** components.

> ⚠️ **Note:** Avoid adding custom colors directly to components. We manage colors globally via `global.css` using **tweakcn**.

Setup:

```bash
cd heritage_graph_ui
npm install
npm run dev
```

Access the app at:

- Landing page → [http://localhost:3000](http://localhost:3000)
- Dashboard → [http://localhost:3000/dashboard](http://localhost:3000/dashboard)

---

## ⚙️ Backend

The backend is powered by **Django REST Framework** and uses **Clerk.com** for authentication.

> ⚠️ **Note:** Make sure to set up the required `.env` file (see `.env.example`).

Setup:

```bash
cd .. # Make sure you are in main directory
python -m venv .myvenv
source .myvenv/bin/activate  # Linux/Mac
pip install uv
uv pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
```

Create a superuser (optional, for admin access):

```bash
python manage.py createsuperuser
```

Run the backend:

```bash
python manage.py runserver
```

Access the backend at:

- API → [http://37.27.182.103:8000](http://37.27.182.103:8000)
- Admin dashboard → [http://37.27.182.103:8000/admin](http://37.27.182.103:8000/admin) (use superuser credentials)

---

## 🤝 Contributing

- Start from the `v1` branch.
- Open an issue or submit a PR with improvements.

---

## 📜 License

The license for this project is yet to be finalized. We’ll choose one that both empowers the community and benefits this project :-)
# testHeritage
