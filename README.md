# bibliograph
An experimental RESTful web API that allow to CRUD operation through HTTP request

## APIs

### Questions

| Method | End Point | Description
|--------|-----|-------------
| GET    | `api/books`     | GET all questions
| GET    | `api/books/:qID` | GET specific question
| POST   | `api/books`     | POST specific question
| PUT    | `api/books/:qID` | UPDATE specific question
| DELETE | `api/books/:qID` | DELETE specific question

--------------------------------------------------------------------------------

## Data Models

### Book

```js
	title:{
		type: String,
		required: true
	},
	genre:{
		type: String,
		required: true
	},
	description:{
		type: String
	},
	author:{
		type: String,
		required: true
	},
	publisher:{
		type: String
	},
	pages:{
		type: String
	},
	image_url:{
		type: String
	},
	buy_url:{
		type: String
	},
	create_date:{
		type: Date,
		default: Date.now
	}
```

### Genre

```js
	name:{
		type: String,
		required: true
	},
	create_date:{
		type: Date,
		default: Date.now
	}
```

