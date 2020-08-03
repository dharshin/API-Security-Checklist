# API Security Checklist
This is a simplified security checklist for anyone who's developing and deploying APIs

---
## Design
- [ ] Make sure that all the RESTful APIs have Swagger definitions (e.g. `format`, `maximum`, `minimum`, `minItems`, `maxItems`) [See Swagger documentation for more information](https://swagger.io/docs/specification/describing-parameters/)
- [ ] Make sure Swagger definitions contain input validation and all expected header parameters
- [ ] Use an API gateway to expose APIs 

## Input Validation

- [ ] Validate user supplied input in the headers and in the body before they are processed
- [ ] Validate the type (e.g. integer, string, floating point number), size (e.g. minimum string lengths, minimum abd maximum values for numbers) and format the composition of expected inputs
- [ ] Use built-in libraries or annotations for input validation as much as possible, build custom validators if built-in functionality is inadequate 
- [ ] Validate the size of the request body and request headers (at the API gateway)
- [ ] Validate the 


## Access Control

## Security Configuration

## Logging 
- [ ] Do not log entire the HTTP request or the HTTP headers or the entire request body as they can potentially contain sensitive information
- [ ] Do not log user and system credentials 
- [ ] Do not log session information

## Build
- [ ] Use third-party components that do not have vulnerabilities

## Monitoring

## Security Testing
- Make sure to incorporate security testing into CI/CD processes
- [ ] Make sure that static application security testing (SAST) is performed in the IDE and in CI (continuous integration)
- [ ] 

