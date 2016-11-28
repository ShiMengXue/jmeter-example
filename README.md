# jmeter-example
Example maven project for jmeter.

The jmeter jmx file must live under src/test/jmeter

To run use "mvn clean verify".  You can also specify properties on the command line e.g. "mvn clean verify -Dtest.threads=100"

Note this example was made using a sample REST api using https://www.npmjs.com/package/json-server.  My server was running this sample JSON:

{
  "posts": [
    { "id": 1, "title": "json-server", "author": "typicode"}, 
    { "id": 2, "title": "Big Shaner's post", "author": "Shaner" }
  ],
  "comments": [
    { "id": 1, "body": "some comment", "postId": 1 },
    { "id": 2, "body": "some comment for shaner's post", "postId": 2 }
  ],
  "profile": { "name": "typicode" }
}
