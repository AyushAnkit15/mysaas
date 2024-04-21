PIXELLNOVATE
Objective: To design and implement an image generator interfacing OPEN AI APIs


Frontend Link : https://github.com/AyushAnkit15/mysaas
https://app.netlify.com/sites/beamish-biscotti-f74477/overview


Technologies Used
MERN STACK : 
Frameworks  :React Js , Express JS, Tailwind
JavaScript Runtime(backend) :Node Js 
Database  :MongoDB

Languages Used
JavaScript

Build Setup
git clone https://github.com/AyushAnkit15/mysaas(backend)
git clone https://github.com/AyushAnkit15/mysaas/tree/master(frontend)

cd server  (for backend only)


Install Dependencies
npm install

Server at localhost:8080
npm run dev(frontend start)
npm start(backend )

API Endpoints

PROMPT AND IMAGE API : 
Request should be made to this api endpoint to generate images.The required headers and request format are : 


GET /api/v1/dal;e
POST /api/v1/dale

POST / api/v1/dalle:
•	Header:
•	Content-Type: application/json
•	Request:
•	Method: POST
•	Endpoint: /api/v1/dalle
•	BODY : 

{
  "prompt": "Text prompt for generating image"
}

•	RESPONSE : 
•	Status Code: 200 OK (for successful response)
•	Body:{ 
  "photo": "Base64 encoded image data"
}
•	Error Response:
•	Status Code: 500 Internal Server Error (for error response)
•	Body
{
  "error": {
    "message": "Error message",
    "code": "Error code" 
•	    // Additional error information if available
  }
}

GALLERY API : 
Request should be made to this api endpoint to get access to gallery and post pictures in the gallery.The required headers and request format are : 
1.	Header:
•	Content-Type: application/json
2.	GET / Endpoint:
•	Request:
•	Method: GET
•	Endpoint: /api/v1/post
•	Response:
•	Status Code: 200 OK (for successful response)
•	Body:  "data": [
    {
      "_id": "Post ID",
      "name": "Name of the post",
      "prompt": "Prompt for the post",
      "photo": "URL of the photo"
    },
    // Additional posts...
  ]
}
•	Error Response:
•	Status Code: 500 Internal Server Error (for error response)
•	Body:
{
  "success": false,
  "message": "Fetching posts failed, please try again"
}
•	POST / api/v1/post:
•	Request:
•	Method: POST
•	Endpoint: /
•	Body: {
  "name": "Name of the post",
  "prompt": "Prompt for the post",
  "photo": "Base64 encoded image data"
}
•	Response:
•	Status Code: 200 OK (for successful response)
•	Body
{
  "success": true,
  "data": {
    "_id": "Post ID",
    "name": "Name of the post",
    "prompt": "Prompt for the post",
    "photo": "URL of the uploaded photo"
  }
•	}
Error Response:
Status Code: 500 Internal Server Error (for error response)
Body:


{
  "error": "Error object",
  "success": false,
  "message": "Unable to create a post, please try again"
}




Connect @
LinkedIn: https://www.linkedin.com/in/ayush-ankit-0536091bb/
Leetcode: https://leetcode.com/AyushAnkit15/
Email: 593ayush.2020@gmail.com
Personal
Name: Ayush Ankit

Gratitude
Thank You
