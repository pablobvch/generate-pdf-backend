# PDF Generator with Node.js

This project is an example of how to generate PDF files from HTML templates using Node.js, Express, and the `html-pdf` library. It was developed for educational purposes to learn about handling HTTP requests, generating PDF files, and integrating web services.

## Objectives

- Create a simple web server with Node.js and Express.
- Generate PDF files from HTML templates.
- Provide a REST API for creating and downloading PDF files.

## Dependencies

This project uses the following dependencies:

- `express`: A minimalist web framework for Node.js.
- `body-parser`: Middleware for parsing the body of HTTP requests.
- `cors`: Middleware for enabling Cross-Origin Resource Sharing.
- `html-pdf`: A library to convert HTML to PDF.
- `phantomjs-prebuilt`: A prebuilt version of PhantomJS, a headless browser used by `html-pdf`.

## Endpoints

### POST /create-pdf

This endpoint is used to create a PDF file from an HTML template. The HTML template is specified in the request body.

**Request Body**:

- `name`: The name of the item.
- `price1`: The first price of the item.
- `price2`: The second price of the item.
- `receiptId`: The receipt ID.

**Response**:

- On success: A JSON object with a message indicating the PDF was created successfully.
- On error: A JSON object with an error message.

### GET /fetch-pdf

This endpoint is used to download the generated PDF file.

**Response**:

- The generated PDF file.

## How to Run

1. Install the project dependencies:

```
npm install
```

2. Start the server:

```
npm start
```


3. The server will start listening on the port specified in the `PORT` environment variable or port 3035 by default.



