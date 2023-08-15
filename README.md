# E-Commerce API


## Description
This is an E-commerce API made using Node.Js, Express & MongoDB. 

## How to setup in your local system
1) Clone the git repository
2) To install all the dependencies, run `npm init` command on terminal in this projects directory
3) Start the server using `node app.js`
4) App starts running on localhost:3000

## How to use the API 
### View all the products
1) Open postman
2) Make a GET request on `localhost:3000/products`
3) All the products with quantities are displayed
![image](https://github.com/ujwalathatavarthi/E-Commerce_API/assets/44131903/a513c4ba-a529-4fbf-abf2-323e86d4e47a)


### To create a new product
1) Open postman
2) Make a POST request on `localhost:3000/products/create`
3) Select Body tab below the url textarea and then select x-www-form-urlencoded
4) Add name & quantity as the keys and set the desired values for the keys.
6) You receive a success message 'New product added successfully.'
7) New product is added to the list.
![image](https://github.com/ujwalathatavarthi/E-Commerce_API/assets/44131903/f1b03705-26ce-4984-96b2-6de505c8e984)


### To delete a product
1) Copy the object id of the product you want to delete.
2) Make a DELETE request using `localhost:3000/products/:id`
3) You will recieve a message saying 'deleted successfully'.
![image](https://github.com/ujwalathatavarthi/E-Commerce_API/assets/44131903/888b1b74-0736-4129-826a-c19edaef0cc1)


### To update the quantity of a product
1) Copy the object id of the product whose quantity you want to update
2) Make a POST request on `localhost:3000/products/:id/update_quantity/?number={x}` where id=object_id and x = increment/decrement value
3) x should be positive for incrementing and negative incase of decrementing.
![image](https://github.com/ujwalathatavarthi/E-Commerce_API/assets/44131903/7f0ae080-393b-44ed-820f-44352aa9547d)






