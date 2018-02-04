# `server/` folder requirements
### Directory structure
- `database/` - Contains `items.json` file with the following schema:

```json
{
	"items": [
		{
			"name": "item1",
			"img": "http://image.url/"
		}
	]
}
```

### Modules

- `index.js` - Includes all other files.
- `./server.js` - Main server executable. Starts Expressjs server. Exports `app` to other modules.
- `./routes.js` - Contains expressjs routing system
- `./pug.js` - Enables Pug.js support for Expressjs server.


```
./index {
  ./server, 
  ./routes {
	./server
  },
  ./pug {
	./server
  }
}
```