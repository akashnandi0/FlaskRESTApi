# FlaskRESTApi
BOOKSTORE PROJECT USING FLASK RESTPLUS APIS
Framework - Flask RESTPlus	Database - MongoDB	
APIs - Requests and Responses :	

Request Method : GET (Search Fields - Author Name, Author Book using parameters)
Url - http://127.0.0.1:5000/api/v1/book/booklist   (Complete List of Books)
Url - http://127.0.0.1:5000/api/v1/book/booklist/<ObjectId> (Particular Book)
Response - status 200 ok

Request Method : POST
Url -  http://127.0.0.1:5000/api/v1/book/bookadd
Body - {
	“book_name”:”Harry Potter”,
“pub_date”:”2021-01-03T11:33:00Z”,
	“author_name”:”J K Rowling”
	}
Response - status 201 created


Request Method : PUT
Url -  http://127.0.0.1:5000/api/v1/book/bookupdate/<ObjectId>
Body - {
	“book_name”:”Harry Potter”,
“pub_date”:”2021-01-03T11:33:00Z”,
	“author_name”:”J K Rowling”
	}
Response - status 200 ok


Request Method : PATCH
Url -  http://127.0.0.1:5000/api/v1/book/bookupdate/<ObjectId>
Body - {
	“book_name”:”Harry Potter”,
	“author_name”:”J K Rowling”
	}
Response - status 200 ok


Request Method : DELETE
Url - http://127.0.0.1:5000/api/v1/book/bookdelete/<ObjectId>
Response - status 204 no content


Additional Features - Searching list of books by using author name or book name
