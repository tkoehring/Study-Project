# Full-Stack Development Study Plan

**Duration:** 6 weeks (can be condensed to 4 if time is tight)  
**Pace:** 2–4 hrs/day, 5 days/week  
**Goal:** Build foundational backend + frontend skills and deploy a full-stack ML web app as a portfolio project.

---

## 📅 Week 1 – Backend Foundations (Flask + FastAPI)

### Topics
- HTTP basics (requests, responses, REST principles)  
- Flask essentials: routing, templates, request handling, JSON APIs  
- FastAPI essentials: async support, request validation with Pydantic, auto-docs with OpenAPI/Swagger  

### Resources
- [Flask Mega-Tutorial (Miguel Grinberg)](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)  
- [FastAPI Official Docs](https://fastapi.tiangolo.com/)  
- YouTube: [Tech With Tim – Flask Tutorial](https://www.youtube.com/watch?v=Z1RJmh_OqeA)  

### ✅ Checkpoint
- Build a small Flask API with 2 endpoints:  
  1. `/predict` → dummy ML prediction (hardcoded output)  
  2. `/health` → returns `"ok"`  

---

## 📅 Week 2 – Backend Expansion (Databases + Auth)

### Topics
- SQL basics with SQLite/Postgres  
- Using SQLAlchemy ORM  
- FastAPI dependency injection  
- JWT-based authentication basics  

### Resources
- [FastAPI with SQLAlchemy Tutorial](https://fastapi.tiangolo.com/tutorial/sql-databases/)  
- [SQLAlchemy ORM Quickstart](https://docs.sqlalchemy.org/en/20/orm/quickstart.html)  
- YouTube: [JWT Auth with FastAPI](https://www.youtube.com/watch?v=0D5EEKH97NA)  

### ✅ Checkpoint
- Extend your API with a database-backed `/users` endpoint  
- Add JWT login/logout routes  

---

## 📅 Week 3 – Frontend Foundations (React.js)

### Topics
- JavaScript + ES6 refresher  
- React basics: components, props, state  
- React Router basics (multi-page navigation)  
- Fetch API / Axios for backend communication  

### Resources
- [React Official Tutorial](https://react.dev/learn)  
- [freeCodeCamp React Full Course](https://www.youtube.com/watch?v=bMknfKXIFA8)  
- [Axios Docs](https://axios-http.com/)  

### ✅ Checkpoint
- Build a React app with:  
  - A login page (connects to FastAPI JWT)  
  - A dashboard page fetching `/predict` results  

---

## 📅 Week 4 – Frontend Expansion (UI + State Mgmt)

### Topics
- Component libraries (Material UI, Ant Design, or Tailwind)  
- Global state management (Context API or Redux basics)  
- Form handling and validation  

### Resources
- [Material UI React](https://mui.com/)  
- [Redux Toolkit](https://redux-toolkit.js.org/tutorials/quick-start)  
- YouTube: [React Context vs Redux](https://www.youtube.com/watch?v=35lXWvCuM8o)  

### ✅ Checkpoint
- Improve dashboard UI with Material UI  
- Add a form for submitting custom inputs → forward request to FastAPI → show predictions in UI  

---

## 📅 Week 5 – Integration + Deployment

### Topics
- CORS setup between React and FastAPI  
- Dockerizing React + FastAPI (multi-container with docker-compose)  
- Serving React build via Nginx reverse proxy  
- AWS/GCP/Heroku deployment basics  

### Resources
- [Dockerizing React + FastAPI Guide](https://testdriven.io/blog/fastapi-react/)  
- [Nginx Reverse Proxy Setup](https://www.nginx.com/resources/wiki/start/topics/examples/reverseproxy/)  
- YouTube: [Deploy FastAPI on AWS EC2](https://www.youtube.com/watch?v=Zp4MuPjpwGA)  

### ✅ Checkpoint
- Deploy your full-stack ML app to AWS EC2 (or Heroku free tier)  
- Verify API + frontend integration live  

---

## 📅 Week 6 – Capstone Full-Stack ML Web App

### Project: **ML Model Dashboard**
- **Backend (FastAPI):** Hosts trained ML model (use your earlier scikit-learn model).  
- **Frontend (React):** Dashboard for inputting data + viewing predictions.  
- **Database:** Store user accounts + prediction history.  
- **Deployment:** Dockerized and hosted on AWS (EC2, EKS, or Elastic Beanstalk).  

### ✅ Deliverables
- GitHub repo with:  
  - `/backend` (FastAPI code, Dockerfile)  
  - `/frontend` (React code, Dockerfile)  
  - `docker-compose.yml`  
  - `README.md` with setup + screenshots  
- Resume bullet:  
  > “Built and deployed a full-stack ML web app using FastAPI (backend), React (frontend), Docker, and AWS, enabling real-time predictions with user authentication and history logging.”  

---
