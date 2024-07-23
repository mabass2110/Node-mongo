
# Node.js Express MongoDB Demo

This is a simple Node.js application using Express.js to provide a RESTful API interface for interacting with MongoDB. It demonstrates basic CRUD operations (Create, Read) with a MongoDB database.

## Prerequisites

Before running this application, make sure you have the following installed:

- Node.js
- npm (Node Package Manager)
- MongoDB (either installed locally or accessible via a remote server)

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd node-express-mongodb-demo
   ```

2. Install dependencies:
   ```
   npm install
   ```

## Configuration

Ensure MongoDB is running and accessible. Modify the `url` variable in `app.js` to match your MongoDB connection string.

```javascript
var url = 'mongodb://mongo:27017/dockerdemo';
```

Replace `'mongodb://mongo:27017/dockerdemo'` with your MongoDB connection URL if necessary.

## Running the Application

To start the application, run:
```
node app.js
```

This will start the Node.js server on `http://localhost:3000`.

## Endpoints

### GET /

Returns a greeting message from the server.

Example:
```
curl http://localhost:3000/
```

### GET /createMongo

Creates a new MongoDB document with a random name and email address in the `customers` collection.

Example:
```
curl http://localhost:3000/createMongo
```

### GET /readMongo

Fetches all documents from the `customers` collection in MongoDB.

Example:
```
curl http://localhost:3000/readMongo
```


## Contributing

Feel free to contribute to this project. You can fork the repository and submit pull requests for any features or fixes you'd like to add.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with Node.js, Express.js, and MongoDB.
- Inspiration and guidance from various online tutorials and documentation.

---

This README provides an overview of how to set up and run your Node.js application using Express.js with MongoDB integration. Customize and expand upon it as needed for your specific project requirements.
