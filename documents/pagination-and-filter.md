# How to pagination and filter post

To pagination and filter post , you can use below query params

| Query param | Description | Default value |
| ----------- | ----------- | ----------- |
| search | Show posts based on a keyword search |
| limit | Number of post to show per page | 10 |
| page | Current page number | 1 |
| orderby | Sort retrieved posts by parameter | 'date' |
| order | Designates the ascending or descending order of the orderby parameter | 'DESC' |
| categories | Show posts associated with certain categories name |
| tags | Show posts associated with certain tags name |

### Example 
- get posts with keyword search hello
```curl
curl --location 'http://localhost/wp-json/root/v1/post?search=hello'
```

- get posts with categories name test
```curl
curl --location 'http://localhost/wp-json/root/v1/post?categories=test'
```

- get first five posts with keyword search
```curl
curl --location 'http://localhost/wp-json/root/v1/post?limit=5&search=hello'
```

For more information [click here](https://developer.wordpress.org/reference/classes/wp_query)
