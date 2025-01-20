
# Review Extractor

## About the Project

The **Review Extractor** is an API server designed to dynamically extract reviews from product pages across different e-commerce platforms, such as Shopify and Amazon. By leveraging modern browser automation frameworks and integration with Large Language Models (LLMs), this project simplifies the process of collecting, structuring, and analyzing product reviews.

---

## Key Features

1. **Dynamic Extraction**  
   - Utilizes AI to dynamically identify CSS selectors for reviews on any given product page. This enables the API to work universally across platforms without hardcoding selectors.

2. **Pagination Handling**  
   - Automatically detects and navigates through paginated review sections to ensure comprehensive data collection.

3. **Scalable and Efficient**  
   - Built using lightweight and scalable technologies like FastAPI, ensuring fast response times and smooth handling of concurrent requests.

4. **AI Integration**  
   - Incorporates OpenAI's GPT model to analyze page structures and determine the appropriate selectors for extracting review data dynamically.

5. **Structured JSON Output**  
   - Provides review data in a clean and standardized JSON format, suitable for further analysis or direct use in applications.

6. **Error Handling**  
   - Robust error handling to gracefully manage invalid URLs, failed extractions, and unexpected scenarios.

7. **Flexible Deployment**  
   - Can be deployed locally or on cloud platforms with minimal configuration, making it accessible to a wide range of users.

---

## Motivation

The motivation behind this project is to simplify and automate the process of collecting product reviews for websites, marketers, and analysts. By providing an API-based solution, users can focus on leveraging the extracted data instead of spending time on manual data collection.

---

## Workflow and System Architecture  

The **system workflow** operates as follows:

1. **Request Submission**:  
   - The user submits a request to the API endpoint with the product page URL.  

2. **Review Extraction**:  
   - The API processes the incoming request by:
     - Fetching the product page using a headless browser.
     - Using AI to identify CSS selectors for review data.
     - Navigating through paginated reviews (if present).
   
3. **Response Delivery**:  
   - The API returns a structured JSON response containing extracted reviews and relevant metadata.

4. **Client Usage**:  
   - Users can directly consume the response for analysis, reporting, or integration into other systems.

---

## Steps to Get and Run the Project

### Prerequisites

Ensure the following are installed on your system:

- **Python** (version 3.8 or higher)  
- **pip** (Python package manager)  
- **Node.js** (required for Playwright)  
- **Git** (for cloning the repository)

### Steps to Run Locally

1. **Clone the Repository**  
   ```bash
   git clone <repository-url>
   cd <repository-folder>




## Sample Respones
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







