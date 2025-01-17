# Inventory with Elasticsearch and Pytest

Welcome to the **Inventory with Elasticsearch and Pytest** project! This repository features a straightforward inventory management system that leverages Elasticsearch for efficient data indexing and searching, and employs Pytest for robust testing of the application's functionality.

---

## Overview

This project implements a simple inventory management system that utilizes Elasticsearch to index and search inventory items. It enables users to perform CRUD (Create, Read, Update, Delete) operations on inventory items and integrates Elasticsearch for efficient searching. The project also includes tests written using Pytest to verify the correctness of the implementation.

---

## Features

- **CRUD Operations**: Perform Create, Read, Update, and Delete operations on inventory items.
- **Elasticsearch Integration**: Leverage Elasticsearch to store and search inventory data efficiently.
- **Pytest for Testing**: Ensure the reliability of the application through unit and integration tests.

---

## Technologies Used

- **Python 3.7+**: The backend of the application is built using Python 3.7 or higher.
- **Elasticsearch**: Used as the primary search engine to store and search inventory items.
- **Pytest**: Testing framework used for writing unit and integration tests.
- **Django**: Web framework used to build the application.
- **Django REST Framework (DRF)**: Facilitates the creation of RESTful APIs.
- **Poetry**: Dependency management tool for Python.
- **Docker**: Used for containerizing the application and services.

---

## Requirements

To run this project, you need the following tools and libraries:

- **Python 3.7+**: Ensure Python 3.7 or higher is installed.
- **Elasticsearch**: You should have an Elasticsearch instance running. You can download and set it up from the [official website](https://www.elastic.co/downloads/elasticsearch).
- **Poetry**: Python dependency management tool. Install it from [Poetry's documentation](https://python-poetry.org/docs/).
- **Docker**: To containerize and run the application services.

---

## Installation

Follow these steps to set up the project locally:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/SahilMehdiyev/Inventory-with-Elasticsearch-and-Pytest.git
   cd Inventory-with-Elasticsearch-and-Pytest
   ```

2. **Install dependencies using Poetry**:
   ```bash
   poetry install
   ```

3. **Set up the environment**:
   - Create a `.env` file in the project root directory and add the necessary environment variables.
   - Refer to `.env.example` for the required variables.

4. **Start Elasticsearch using Docker**:
   Ensure Docker is installed and running on your system. Use the provided `docker-compose.yml` to start the Elasticsearch service:

   ```bash
   docker-compose up -d
   ```

5. **Apply database migrations**:
   ```bash
   poetry run python manage.py migrate
   ```

6. **Create a superuser** (optional, for accessing the Django admin interface):
   ```bash
   poetry run python manage.py createsuperuser
   ```

7. **Start the development server**:
   ```bash
   poetry run python manage.py runserver
   ```

---

## Usage

Once the server is running, you can:

- Access the API endpoints to perform CRUD operations on inventory items.
- Use the Django admin interface to manage inventory items.
- Utilize Elasticsearch to search for inventory items efficiently.

---

## Testing

To run the tests using Pytest:

```bash
poetry run pytest
```

Ensure that the Elasticsearch service is running before executing the tests.

---

## Contributing

Contributions are welcome! If you have ideas for new features or improvements, feel free to:

1. Fork the repository.
2. Create a new branch for your feature or bugfix.
3. Submit a pull request.

Please ensure your contributions align with the project's goals and maintain clean, modular code.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact

For questions, suggestions, or feedback, feel free to reach out:

- **Author**: Sahil Mehdiyev
- **Email**: [branchsahil@gmail.com](mailto:branchsahil@gmail.com)
- **GitHub**: [SahilMehdiyev](https://github.com/SahilMehdiyev)

---

Happy managing your inventory! 🚀
