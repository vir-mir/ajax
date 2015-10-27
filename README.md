
Ajax examples
--------------

```javascript
ajax.get('example.com')
	 .then(function(response){
		alert(response);
	 });
```

```javascript
ajax.put('example.com',{
		firstname: 'Pedro',
		lastname: 'Sanchez',
		age: 30
	 })
	 .then(function(response){
		// Make some useful actions
	 })
	 .catch(function(e,url){
		// Process the error
	 });
```

Basics
------

```javascript
ajax.<method>(<url>,[data],[options])
	 .then(function(response){
		// Run when the request is successful
	 })
	 .catch(function(e,url){
		// Process the error
	 })
	 .complete(function(){
		// Always run
	 });
```
