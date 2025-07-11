# country-capital-api

## What

`country-capital-api` is a lightweight, Python-based REST API built with Flask that returns the name of a country when provided with the name of its capital city.

The API is designed to be used as a microservice and can be easily integrated into other applications within the organization.

A live microservice endpoint is also available at:

```
https://example.com/country-capital/<query-params>
```

---

## How to set up a local development environment

Follow these steps to set up and run the API locally:

1. **Clone the repository**

```bash
git clone https://github.com/your-org/country-capital-api.git
cd country-capital-api
```

2. **Create and activate a virtual environment (recommended)**

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

4. **Run the API server**

```bash
uvicorn app:app --reload
```

By default, the server will be available at:

```
http://127.0.0.1:8000
```

---

## Prerequisites

* **Python 3.8+**: Make sure Python is installed on your system.
* **pip**: Python package manager for installing dependencies.
* **Uvicorn**: ASGI server for running the Flask application.

---

## Example Usage

Once running, you can query the API by providing the capital city as a parameter.

**Request:**

```
GET http://127.0.0.1:8000/country-capital?city=Berlin
```

**Response:**

```json
{
  "country": "Germany"
}
```

