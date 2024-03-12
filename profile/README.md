### Fidesy Pay

Like stripe but only with crypto

description todo...

Current microservices [dependencies](http://45.95.11.245:16686/dependencies) 
![](https://github.com/fidesy-pay/.github/blob/master/images/graph.png)

### Frontend endpoints 

* Sign up http://45.95.11.245:4000/signup

* Login http://45.95.11.245:4000/login

* Profile http://45.95.11.245:4000/profile

* Invoice http://45.95.11.245:4000/invoices/invoice-uuid

### GraphQL

http://45.95.11.245:7090

### Tracing Jaeger

http://45.95.11.245:16686/search

### Logs Graylog

http://45.95.11.245:9000

### How to create invoice

1. Sign up user
2. Get api key from /profile endpoint

```curl -X POST http://45.95.11.245:7090/api/invoice -H 'api-key: <API_KEY>' -d '{"usd_amount": 5.99}'```

