#  FedEx Delivery Optimizer

A multi-agent workflow system built with **LangGraph**, **FastAPI**, and **Streamlit** for intelligent delivery route optimization.

![FedEx Delivery Optimizer Dashboard](https://via.placeholder.com/800x400/2563eb/ffffff?text=FedEx+Delivery+Optimizer+Dashboard)

##  Architecture

- **Backend**: FastAPI with LangGraph workflow orchestration
- **Frontend**: Streamlit dashboard for order creation and route visualization
- **Agents**: Order Ingestion, Geocoding, Route Optimization
- **Database**: PostgreSQL (optional - works with mock data)

### 1. Install Dependencies

```bash
# Backend dependencies
cd Backend
pip install -r requirements.txt

# Frontend dependencies
cd ../Frontend
pip install streamlit requests
```

### 2. Start the Backend

```bash
cd Backend
uvicorn main:app --reload --host 0.0.0.0 --port 8000
```

### 3. Start the Frontend

```bash
cd Frontend
streamlit run app.py
```

### 4. Access the Application

- **Frontend**: http://localhost:8501
- **Backend API**: http://localhost:8000
- **API Docs**: http://localhost:8000/docs

## Workflow

1. **Order Ingestion**: Creates order in database
2. **Geocoding**: Converts address to coordinates
3. **Route Optimization**: Generates optimal delivery routes

## 📊 Features

-  Multi-agent LangGraph workflow
-  Real-time order processing
-  Route visualization
-  Error handling and fallbacks
-  Mock data support (works without database)

## 🛠️ Tech Stack

- **LangGraph**: Workflow orchestration
- **FastAPI**: Backend API
- **Streamlit**: Frontend dashboard
- **PostgreSQL**: Database 
- **SQLAlchemy**: ORM




## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [LangGraph](https://github.com/langchain-ai/langgraph) for workflow orchestration
- [FastAPI](https://fastapi.tiangolo.com/) for the modern web framework
- [Streamlit](https://streamlit.io/) for the interactive dashboard
- [OR-Tools](https://developers.google.com/optimization) for route optimization algorithms

---

**Built with ❤️ using LangGraph, FastAPI & Streamlit**
