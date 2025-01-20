


# Review Extracter

## Project Description

The Review Extractor is an API server designed to extract reviews from any product page (e.g., Shopify, Amazon) in JSON format. It automates the process of retrieving review data, making it convenient for websites to manage and analyze feedback efficiently.

## Motivation

The motivation behind this project is to provide a simple and efficient way to collect reviews data in json form for websites.

## System Architecture or Workflow

The operational flow of the project can be summarized as follows:

- A user sends a request to the API endpoint with the product page URL.
- The API processes the request, extracting the necessary review details.
- The extracted information is returned to the user in the form of a structured response.

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
