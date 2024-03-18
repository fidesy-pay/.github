### Fidesy Pay

Like stripe but only with crypto

description todo...

Current microservices [dependencies](http://tracing.fidesy.tech/dependencies) 
![](https://github.com/fidesy-pay/.github/blob/master/images/graph.png)

### Frontend endpoints 

* Sign up http://pay.fidesy.tech/signup

* Login http://pay.fidesy.tech/login

* Overview http://pay.fidesy.tech/overview

* Profile http://pay.fidesy.tech/profile

* Invoice http://pay.fidesy.tech/invoices/invoice-uuid

### GraphQL

http://facade.pay.fidesy.tech

### Tracing Jaeger

http://tracing.fidesy.tech/search

### Logs Graylog

http://logging.fidesy.tech

### How to create invoice

1. Sign up user
2. Get api key from /profile endpoint

```curl -X POST http://facade.pay.fidesy.tech/api/invoice -H 'api-key: <API_KEY>' -d '{"usd_amount": 5.99}'```

