### Chaining array methods

Get an array containing only the names of courses from Framework.

```js
    var courses = [
    	{
    		name: 'Redux',
    		type: 'Libraries'
    	},
    	{
    		name: 'React',
    		type: 'Framework'
    	},
    	{
    		name: 'Angular',
    		type: 'Framework'
    	},
    	{
    		name: 'Apollo',
    		type: 'Libraries'
    	},
    	{
    		name: 'MobX',
    		type: 'Libraries'
    	}
    ];
```

Use Array.filter() to reduce the list to only courses in Framework, and then Array.map() to create a new array of only names.

```js
    var framework = courses.filter(function (course) {
    	return course.type === 'Framework';
    }).map(function (course) {
    	return course.name;
    });
```
