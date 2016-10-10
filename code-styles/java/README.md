JAVA
====

Coding conventions
------------------
1. Groovy
	1. Use TABS only for identation
	2. Use spacing generously
	3. Don't declare anything `public`. By default they already are
	4. Use `==` instead of `equals()`
	5. Don't create getter/setters. By default Groovy generates these
	6. Have a space before and after operators: `((a + b) / 3) % 2) == 0`
	7. Have a space after commas: `method(1, 2, 3)`
	8. Always declare `@CompileStatic` at the class unless for good reasons
	9. Always declare types for variables and methods if they are not inferable:
		1. `List<User> users = []`
		2. `def users = userRepo.findUsers()` - OK, can infer return type of `findUsers()`
		3. `Map<Long, User> id2Users = [:]`
	10. Use string interpolation as much as possible: `println("Hello ${user.name}");`
	11. When passing in closures don't need to have brackets: `items.each { println(it); }`
	12. However, when there is a chain of closures, use brackets for clarity: `items.findAll({ it.name != null }).collect({ it.name }).each({ println(it); })`
2. HTML
	1. Use TABS also
	2. Use double quotes `"` for quoting attributes
	3. Always close all tags: `<br/>`
3. JavaScript
	1. Plain JavaScript with jQuery is fine for this project 
	2. Save `this` to make code clearer: `var self = this;`
	3. Try to include `<scripts>` from some CDN