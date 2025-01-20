


# Review Extracter

## Project Description

API server capable of extracting reviews information from any given product page (e.g., Shopify, Amazon).

## Motivation

The motivation behind this project is to provide a simple and efficient way to collect reviews data in json form for websites.

## System Architecture or Workflow

System Architecture or Workflow

- The user submits a request to the API's endpoint.
- The API processes the incoming request and generates a response.
- The processed response is sent back to the user.

## API Usage and Sample Responses

The API provides the following endpoints:

* `GET /reviews/`: Returns a list of all reviews.
* `POST /reviews/`: Creates a new review.
* `GET /reviews/:id`: Returns a single review by ID.
* `PUT /reviews/:id`: Updates a single review by ID.
* `DELETE /reviews/:id`: Deletes a single review by ID.

Here is an example of a sample response:
{
  "reviews_count": 150,
  "reviews": [
    {
      "title": "Excellent Product!",
      "body": "I have been using this product for a week, and it has exceeded my expectations...",
      "rating": 5,
      "reviewer": "Ankit Kumar"
    },
    {
      "title": "Not worth the price",
      "body": "The product did not perform as advertised. I encountered several issues...",
      "rating": 2,
      "reviewer": "Ashish singh"
    }
   
}

## Instructions on How to Run the Project

To run the project, follow these steps:

1. Clone the repository using `git clone`.
2. Install the required dependencies using `pip install -r requirements.txt`.
3. Run the migrations using `python manage.py migrate`.
4. Start the development server using `python manage.py runserver`.
