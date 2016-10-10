Testing
=======

A guide for writting test for projects.

TBD

Java Testing
------------
1. No JUnit setup yet
2. Simply add test methods in any class
3. Method signature: `void testXXX(List<String> args)`
4. Running the test method: `java -cp classes:lib/* tool.Test className methodName [additional arguments]`
5. Example (make sure Seed is already run): `java -cp classes:lib/* tool.Test repo.UserRepo testFindByUsername`
6. Testing all methods: `java -cp classes:lib/* tool.Test all`
7. No front-end tests yet, perhaps overkill