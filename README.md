# Sample Book Store

This is a simple Spring Boot application for managing a bookstore. The application allows users to perform CRUD operations on books.

## Project Structure

- **.mvn/wrapper**: Maven wrapper files
- **bin**: Compiled binaries
- **src**: Source code of the application
- **.gitignore**: Git ignore file
- **mvnw**: Maven wrapper script
- **mvnw.cmd**: Maven wrapper script for Windows
- **pom.xml**: Maven project file

## Installation

To install and run this project locally, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/sush5757/Bookstore-Rest-api.git
    cd sample-book-store
    ```

2. **Build the project**:
    ```bash
    ./mvnw clean install
    ```

3. **Run the application**:
    ```bash
    ./mvnw spring-boot:run
    ```

## Usage

The application exposes RESTful endpoints to manage books. Below are the available endpoints:

- **GET /books**: Retrieve all books
- **GET /books/{id}**: Retrieve a book by its ID
- **POST /books**: Create a new book
- **PUT /books/{id}**: Update an existing book by its ID
- **DELETE /books/{id}**: Delete a book by its ID

### Sample Requests

- **Retrieve all books**:
    ```bash
    curl -X GET http://localhost:8080/books
    ```

- **Retrieve a book by ID**:
    ```bash
    curl -X GET http://localhost:8080/books/{id}
    ```

- **Create a new book**:
    ```bash
    curl -X POST http://localhost:8080/books -H "Content-Type: application/json" -d '{"title": "Book Title", "author": "Author Name", "isbn": "1234567890"}'
    ```

- **Update an existing book**:
    ```bash
    curl -X PUT http://localhost:8080/books/{id} -H "Content-Type: application/json" -d '{"title": "Updated Title", "author": "Updated Author", "isbn": "0987654321"}'
    ```

- **Delete a book**:
    ```bash
    curl -X DELETE http://localhost:8080/books/{id}
    ```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Create a new Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or issues, please contact [sushantmanjare17269@gmail.com](mailto:sushantmanjare17269@gmail.com).

## Acknowledgements

- Spring Boot
- Maven

## Features

- CRUD operations for books
- Simple RESTful API

## Technologies Used

- Java
- Spring Boot
- Maven
- JPA

## Known Issues/Bugs

- No known issues at this time. Please report any issues in the repository's issue tracker.

## FAQ

**Q: How can I run the tests?**
A: Use the following command to run the tests:
   ```bash
   ./mvnw test
