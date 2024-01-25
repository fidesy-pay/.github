### Fidesy Pay

Like stripe but only with crypto

description todo...

Current microservices [dependencies](http://77.91.123.23:16686/dependencies) 
![](https://github.com/fidesy-pay/.github/blob/master/images/graph.png)

### Frontend endpoints 

* Sign up http://77.91.123.23:4000/signup

* Login http://77.91.123.23:4000/login

* Profile http://77.91.123.23:4000/profile

* Invoice http://77.91.123.23:4000/invoices/invoice-uuid

### GraphQL

http://77.91.123.23:7090

### Tracing Jaeger

http://77.91.123.23:16686/search

### Logs Graylog

http://77.91.123.23:9000

### How to create invoice

1. Sign up user
2. Get api key from /profile endpoint

```curl -X POST http://77.91.123.23:7090/api/invoice -H 'api-key: <API_KEY>' -d '{"usd_amount": 0.001}'```

