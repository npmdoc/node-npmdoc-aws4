# api documentation for  [aws4 (v1.6.0)](https://github.com/mhart/aws4#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-aws4.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-aws4) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-aws4.svg)](https://travis-ci.org/npmdoc/node-npmdoc-aws4)
#### Signs and prepares requests using AWS Signature Version 4

[![NPM](https://nodei.co/npm/aws4.png?downloads=true)](https://www.npmjs.com/package/aws4)

[![apidoc](https://npmdoc.github.io/node-npmdoc-aws4/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-aws4_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-aws4/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-aws4/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Michael Hart",
        "email": "michael.hart.au@gmail.com",
        "url": "http://github.com/mhart"
    },
    "bugs": {
        "url": "https://github.com/mhart/aws4/issues"
    },
    "dependencies": {},
    "description": "Signs and prepares requests using AWS Signature Version 4",
    "devDependencies": {
        "mocha": "^2.4.5",
        "should": "^8.2.2"
    },
    "directories": {},
    "dist": {
        "shasum": "83ef5ca860b2b32e4a0deedee8c771b9db57471e",
        "tarball": "https://registry.npmjs.org/aws4/-/aws4-1.6.0.tgz"
    },
    "gitHead": "74bf0b64d1e8cbcd184964999c7ef53f52d7ad32",
    "homepage": "https://github.com/mhart/aws4#readme",
    "keywords": [
        "amazon",
        "aws",
        "signature",
        "s3",
        "ec2",
        "autoscaling",
        "cloudformation",
        "elasticloadbalancing",
        "elb",
        "elasticbeanstalk",
        "cloudsearch",
        "dynamodb",
        "kinesis",
        "lambda",
        "glacier",
        "sqs",
        "sns",
        "iam",
        "sts",
        "ses",
        "swf",
        "storagegateway",
        "datapipeline",
        "directconnect",
        "redshift",
        "opsworks",
        "rds",
        "monitoring",
        "cloudtrail",
        "cloudfront",
        "codedeploy",
        "elasticache",
        "elasticmapreduce",
        "elastictranscoder",
        "emr",
        "cloudwatch",
        "mobileanalytics",
        "cognitoidentity",
        "cognitosync",
        "cognito",
        "containerservice",
        "ecs",
        "appstream",
        "keymanagementservice",
        "kms",
        "config",
        "cloudhsm",
        "route53",
        "route53domains",
        "logs"
    ],
    "license": "MIT",
    "main": "aws4.js",
    "maintainers": [
        {
            "name": "hichaelmart",
            "email": "michael.hart.au@gmail.com"
        }
    ],
    "name": "aws4",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mhart/aws4.git"
    },
    "scripts": {
        "test": "mocha ./test/fast.js ./test/slow.js -b -t 100s -R list"
    },
    "version": "1.6.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module aws4](#apidoc.module.aws4)
1.  [function <span class="apidocSignatureSpan">aws4.</span>RequestSigner (request, credentials)](#apidoc.element.aws4.RequestSigner)
1.  [function <span class="apidocSignatureSpan">aws4.</span>sign (request, credentials)](#apidoc.element.aws4.sign)
1.  object <span class="apidocSignatureSpan">aws4.</span>RequestSigner.prototype

#### [module aws4.RequestSigner](#apidoc.module.aws4.RequestSigner)
1.  [function <span class="apidocSignatureSpan">aws4.</span>RequestSigner (request, credentials)](#apidoc.element.aws4.RequestSigner.RequestSigner)

#### [module aws4.RequestSigner.prototype](#apidoc.module.aws4.RequestSigner.prototype)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>authHeader ()](#apidoc.element.aws4.RequestSigner.prototype.authHeader)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>canonicalHeaders ()](#apidoc.element.aws4.RequestSigner.prototype.canonicalHeaders)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>canonicalString ()](#apidoc.element.aws4.RequestSigner.prototype.canonicalString)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>createHost ()](#apidoc.element.aws4.RequestSigner.prototype.createHost)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>credentialString ()](#apidoc.element.aws4.RequestSigner.prototype.credentialString)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>defaultCredentials ()](#apidoc.element.aws4.RequestSigner.prototype.defaultCredentials)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>formatPath ()](#apidoc.element.aws4.RequestSigner.prototype.formatPath)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>getDate ()](#apidoc.element.aws4.RequestSigner.prototype.getDate)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>getDateTime ()](#apidoc.element.aws4.RequestSigner.prototype.getDateTime)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>isSingleRegion ()](#apidoc.element.aws4.RequestSigner.prototype.isSingleRegion)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>matchHost (host)](#apidoc.element.aws4.RequestSigner.prototype.matchHost)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>parsePath ()](#apidoc.element.aws4.RequestSigner.prototype.parsePath)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>prepareRequest ()](#apidoc.element.aws4.RequestSigner.prototype.prepareRequest)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>sign ()](#apidoc.element.aws4.RequestSigner.prototype.sign)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>signature ()](#apidoc.element.aws4.RequestSigner.prototype.signature)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>signedHeaders ()](#apidoc.element.aws4.RequestSigner.prototype.signedHeaders)
1.  [function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>stringToSign ()](#apidoc.element.aws4.RequestSigner.prototype.stringToSign)



# <a name="apidoc.module.aws4"></a>[module aws4](#apidoc.module.aws4)

#### <a name="apidoc.element.aws4.RequestSigner"></a>[function <span class="apidocSignatureSpan">aws4.</span>RequestSigner (request, credentials)](#apidoc.element.aws4.RequestSigner)
- description and source-code
```javascript
function RequestSigner(request, credentials) {

  if (typeof request === 'string') request = url.parse(request)

  var headers = request.headers = (request.headers || {}),
      hostParts = this.matchHost(request.hostname || request.host || headers.Host || headers.host)

  this.request = request
  this.credentials = credentials || this.defaultCredentials()

  this.service = request.service || hostParts[0] || ''
  this.region = request.region || hostParts[1] || 'us-east-1'

  // SES uses a different domain from the service name
  if (this.service === 'email') this.service = 'ses'

  if (!request.method && request.body)
    request.method = 'POST'

  if (!headers.Host && !headers.host) {
    headers.Host = request.hostname || request.host || this.createHost()

    // If a port is specified explicitly, use it as is
    if (request.port)
      headers.Host += ':' + request.port
  }
  if (!request.hostname && !request.host)
    request.hostname = headers.Host || headers.host

  this.isCodeCommitGit = this.service === 'codecommit' && request.method === 'GIT'
}
```
- example usage
```shell
...
  }
}))
/*
(HTTP 202, empty response)
*/

// Generate CodeCommit Git access password
var signer = new aws4.RequestSigner({
  service: 'codecommit',
  host: 'git-codecommit.us-east-1.amazonaws.com',
  method: 'GIT',
  path: '/v1/repos/MyAwesomeRepo',
})
var password = signer.getDateTime() + 'Z' + signer.signature()
'''
...
```

#### <a name="apidoc.element.aws4.sign"></a>[function <span class="apidocSignatureSpan">aws4.</span>sign (request, credentials)](#apidoc.element.aws4.sign)
- description and source-code
```javascript
sign = function (request, credentials) {
  return new RequestSigner(request, credentials).sign()
}
```
- example usage
```shell
...

// alternatively (as aws4 can infer the host):
opts = {service: 'sqs', region: 'us-east-1', path: '/?Action=ListQueues'}

// alternatively (as us-east-1 is default):
opts = {service: 'sqs', path: '/?Action=ListQueues'}

aws4.sign(opts) // assumes AWS credentials are available in process.env

console.log(opts)
/*
{
host: 'sqs.us-east-1.amazonaws.com',
path: '/?Action=ListQueues',
headers: {
...
```



# <a name="apidoc.module.aws4.RequestSigner"></a>[module aws4.RequestSigner](#apidoc.module.aws4.RequestSigner)

#### <a name="apidoc.element.aws4.RequestSigner.RequestSigner"></a>[function <span class="apidocSignatureSpan">aws4.</span>RequestSigner (request, credentials)](#apidoc.element.aws4.RequestSigner.RequestSigner)
- description and source-code
```javascript
function RequestSigner(request, credentials) {

  if (typeof request === 'string') request = url.parse(request)

  var headers = request.headers = (request.headers || {}),
      hostParts = this.matchHost(request.hostname || request.host || headers.Host || headers.host)

  this.request = request
  this.credentials = credentials || this.defaultCredentials()

  this.service = request.service || hostParts[0] || ''
  this.region = request.region || hostParts[1] || 'us-east-1'

  // SES uses a different domain from the service name
  if (this.service === 'email') this.service = 'ses'

  if (!request.method && request.body)
    request.method = 'POST'

  if (!headers.Host && !headers.host) {
    headers.Host = request.hostname || request.host || this.createHost()

    // If a port is specified explicitly, use it as is
    if (request.port)
      headers.Host += ':' + request.port
  }
  if (!request.hostname && !request.host)
    request.hostname = headers.Host || headers.host

  this.isCodeCommitGit = this.service === 'codecommit' && request.method === 'GIT'
}
```
- example usage
```shell
...
  }
}))
/*
(HTTP 202, empty response)
*/

// Generate CodeCommit Git access password
var signer = new aws4.RequestSigner({
  service: 'codecommit',
  host: 'git-codecommit.us-east-1.amazonaws.com',
  method: 'GIT',
  path: '/v1/repos/MyAwesomeRepo',
})
var password = signer.getDateTime() + 'Z' + signer.signature()
'''
...
```



# <a name="apidoc.module.aws4.RequestSigner.prototype"></a>[module aws4.RequestSigner.prototype](#apidoc.module.aws4.RequestSigner.prototype)

#### <a name="apidoc.element.aws4.RequestSigner.prototype.authHeader"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>authHeader ()](#apidoc.element.aws4.RequestSigner.prototype.authHeader)
- description and source-code
```javascript
authHeader = function () {
  return [
    'AWS4-HMAC-SHA256 Credential=' + this.credentials.accessKeyId + '/' + this.credentialString(),
    'SignedHeaders=' + this.signedHeaders(),
    'Signature=' + this.signature(),
  ].join(', ')
}
```
- example usage
```shell
...

RequestSigner.prototype.sign = function() {
  if (!this.parsedPath) this.prepareRequest()

  if (this.request.signQuery) {
    this.parsedPath.query['X-Amz-Signature'] = this.signature()
  } else {
    this.request.headers.Authorization = this.authHeader()
  }

  this.request.path = this.formatPath()

  return this.request
}
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.canonicalHeaders"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>canonicalHeaders ()](#apidoc.element.aws4.RequestSigner.prototype.canonicalHeaders)
- description and source-code
```javascript
canonicalHeaders = function () {
  var headers = this.request.headers
  function trimAll(header) {
    return header.toString().trim().replace(/\s+/g, ' ')
  }
  return Object.keys(headers)
    .sort(function(a, b) { return a.toLowerCase() < b.toLowerCase() ? -1 : 1 })
    .map(function(key) { return key.toLowerCase() + ':' + trimAll(headers[key]) })
    .join('\n')
}
```
- example usage
```shell
...
  if (decodeSlashesInPath) pathStr = pathStr.replace(/%2F/g, '/')
}

return [
  this.request.method || 'GET',
  pathStr,
  queryStr,
  this.canonicalHeaders() + '\n',
  this.signedHeaders(),
  bodyHash,
].join('\n')
}

RequestSigner.prototype.canonicalHeaders = function() {
var headers = this.request.headers
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.canonicalString"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>canonicalString ()](#apidoc.element.aws4.RequestSigner.prototype.canonicalString)
- description and source-code
```javascript
canonicalString = function () {
  if (!this.parsedPath) this.prepareRequest()

  var pathStr = this.parsedPath.path,
      query = this.parsedPath.query,
      headers = this.request.headers,
      queryStr = '',
      normalizePath = this.service !== 's3',
      decodePath = this.service === 's3' || this.request.doNotEncodePath,
      decodeSlashesInPath = this.service === 's3',
      firstValOnly = this.service === 's3',
      bodyHash

  if (this.service === 's3' && this.request.signQuery) {
    bodyHash = 'UNSIGNED-PAYLOAD'
  } else if (this.isCodeCommitGit) {
    bodyHash = ''
  } else {
    bodyHash = headers['X-Amz-Content-Sha256'] || headers['x-amz-content-sha256'] ||
      hash(this.request.body || '', 'hex')
  }

  if (query) {
    queryStr = encodeRfc3986(querystring.stringify(Object.keys(query).sort().reduce(function(obj, key) {
      if (!key) return obj
      obj[key] = !Array.isArray(query[key]) ? query[key] :
        (firstValOnly ? query[key][0] : query[key].slice().sort())
      return obj
    }, {})))
  }
  if (pathStr !== '/') {
    if (normalizePath) pathStr = pathStr.replace(/\/{2,}/g, '/')
    pathStr = pathStr.split('/').reduce(function(path, piece) {
      if (normalizePath && piece === '..') {
        path.pop()
      } else if (!normalizePath || piece !== '.') {
        if (decodePath) piece = querystring.unescape(piece)
        path.push(encodeRfc3986(querystring.escape(piece)))
      }
      return path
    }, []).join('/')
    if (pathStr[0] !== '/') pathStr = '/' + pathStr
    if (decodeSlashesInPath) pathStr = pathStr.replace(/%2F/g, '/')
  }

  return [
    this.request.method || 'GET',
    pathStr,
    queryStr,
    this.canonicalHeaders() + '\n',
    this.signedHeaders(),
    bodyHash,
  ].join('\n')
}
```
- example usage
```shell
...
}

RequestSigner.prototype.stringToSign = function() {
return [
  'AWS4-HMAC-SHA256',
  this.getDateTime(),
  this.credentialString(),
  hash(this.canonicalString(), 'hex'),
].join('\n')
}

RequestSigner.prototype.canonicalString = function() {
if (!this.parsedPath) this.prepareRequest()

var pathStr = this.parsedPath.path,
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.createHost"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>createHost ()](#apidoc.element.aws4.RequestSigner.prototype.createHost)
- description and source-code
```javascript
createHost = function () {
  var region = this.isSingleRegion() ? '' :
        (this.service === 's3' && this.region !== 'us-east-1' ? '-' : '.') + this.region,
      service = this.service === 'ses' ? 'email' : this.service
  return service + region + '.amazonaws.com'
}
```
- example usage
```shell
...
// SES uses a different domain from the service name
if (this.service === 'email') this.service = 'ses'

if (!request.method && request.body)
  request.method = 'POST'

if (!headers.Host && !headers.host) {
  headers.Host = request.hostname || request.host || this.createHost()

  // If a port is specified explicitly, use it as is
  if (request.port)
    headers.Host += ':' + request.port
}
if (!request.hostname && !request.host)
  request.hostname = headers.Host || headers.host
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.credentialString"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>credentialString ()](#apidoc.element.aws4.RequestSigner.prototype.credentialString)
- description and source-code
```javascript
credentialString = function () {
  return [
    this.getDate(),
    this.region,
    this.service,
    'aws4_request',
  ].join('/')
}
```
- example usage
```shell
...

if (query['X-Amz-Date'])
  this.datetime = query['X-Amz-Date']
else
  query['X-Amz-Date'] = this.getDateTime()

query['X-Amz-Algorithm'] = 'AWS4-HMAC-SHA256'
query['X-Amz-Credential'] = this.credentials.accessKeyId + '/' + this.credentialString()
query['X-Amz-SignedHeaders'] = this.signedHeaders()

  } else {

if (!request.doNotModifyHeaders && !this.isCodeCommitGit) {
  if (request.body && !headers['Content-Type'] && !headers['content-type'])
    headers['Content-Type'] = 'application/x-www-form-urlencoded; charset=utf-8'
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.defaultCredentials"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>defaultCredentials ()](#apidoc.element.aws4.RequestSigner.prototype.defaultCredentials)
- description and source-code
```javascript
defaultCredentials = function () {
  var env = process.env
  return {
    accessKeyId: env.AWS_ACCESS_KEY_ID || env.AWS_ACCESS_KEY,
    secretAccessKey: env.AWS_SECRET_ACCESS_KEY || env.AWS_SECRET_KEY,
    sessionToken: env.AWS_SESSION_TOKEN,
  }
}
```
- example usage
```shell
...

if (typeof request === 'string') request = url.parse(request)

var headers = request.headers = (request.headers || {}),
    hostParts = this.matchHost(request.hostname || request.host || headers.Host || headers.host)

this.request = request
this.credentials = credentials || this.defaultCredentials()

this.service = request.service || hostParts[0] || ''
this.region = request.region || hostParts[1] || 'us-east-1'

// SES uses a different domain from the service name
if (this.service === 'email') this.service = 'ses'
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.formatPath"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>formatPath ()](#apidoc.element.aws4.RequestSigner.prototype.formatPath)
- description and source-code
```javascript
formatPath = function () {
  var path = this.parsedPath.path,
      query = this.parsedPath.query

  if (!query) return path

  // Services don't support empty query string keys
  if (query[''] != null) delete query['']

  return path + '?' + encodeRfc3986(querystring.stringify(query))
}
```
- example usage
```shell
...

if (this.request.signQuery) {
  this.parsedPath.query['X-Amz-Signature'] = this.signature()
} else {
  this.request.headers.Authorization = this.authHeader()
}

this.request.path = this.formatPath()

return this.request
}

RequestSigner.prototype.getDateTime = function() {
if (!this.datetime) {
  var headers = this.request.headers,
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.getDate"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>getDate ()](#apidoc.element.aws4.RequestSigner.prototype.getDate)
- description and source-code
```javascript
getDate = function () {
  return this.getDateTime().substr(0, 8)
}
```
- example usage
```shell
...
  'AWS4-HMAC-SHA256 Credential=' + this.credentials.accessKeyId + '/' + this.credentialString(),
  'SignedHeaders=' + this.signedHeaders(),
  'Signature=' + this.signature(),
].join(', ')
}

RequestSigner.prototype.signature = function() {
var date = this.getDate(),
    cacheKey = [this.credentials.secretAccessKey, date, this.region, this.service].join(),
    kDate, kRegion, kService, kCredentials = credentialsCache.get(cacheKey)
if (!kCredentials) {
  kDate = hmac('AWS4' + this.credentials.secretAccessKey, date)
  kRegion = hmac(kDate, this.region)
  kService = hmac(kRegion, this.service)
  kCredentials = hmac(kService, 'aws4_request')
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.getDateTime"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>getDateTime ()](#apidoc.element.aws4.RequestSigner.prototype.getDateTime)
- description and source-code
```javascript
getDateTime = function () {
  if (!this.datetime) {
    var headers = this.request.headers,
      date = new Date(headers.Date || headers.date || new Date)

    this.datetime = date.toISOString().replace(/[:\-]|\.\d{3}/g, '')

    // Remove the trailing 'Z' on the timestamp string for CodeCommit git access
    if (this.isCodeCommitGit) this.datetime = this.datetime.slice(0, -1)
  }
  return this.datetime
}
```
- example usage
```shell
...
// Generate CodeCommit Git access password
var signer = new aws4.RequestSigner({
  service: 'codecommit',
  host: 'git-codecommit.us-east-1.amazonaws.com',
  method: 'GIT',
  path: '/v1/repos/MyAwesomeRepo',
})
var password = signer.getDateTime() + 'Z' + signer.signature()
'''

API
---

### aws4.sign(requestOptions, [credentials])
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.isSingleRegion"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>isSingleRegion ()](#apidoc.element.aws4.RequestSigner.prototype.isSingleRegion)
- description and source-code
```javascript
isSingleRegion = function () {
  // Special case for S3 and SimpleDB in us-east-1
  if (['s3', 'sdb'].indexOf(this.service) >= 0 && this.region === 'us-east-1') return true

  return ['cloudfront', 'ls', 'route53', 'iam', 'importexport', 'sts']
    .indexOf(this.service) >= 0
}
```
- example usage
```shell
...
if (['s3', 'sdb'].indexOf(this.service) >= 0 && this.region === 'us-east-1') return true

return ['cloudfront', 'ls', 'route53', 'iam', 'importexport', 'sts']
  .indexOf(this.service) >= 0
}

RequestSigner.prototype.createHost = function() {
var region = this.isSingleRegion() ? '' :
      (this.service === 's3' && this.region !== 'us-east-1' ? '-' : '.') + this.region,
    service = this.service === 'ses' ? 'email' : this.service
return service + region + '.amazonaws.com'
}

RequestSigner.prototype.prepareRequest = function() {
this.parsePath()
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.matchHost"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>matchHost (host)](#apidoc.element.aws4.RequestSigner.prototype.matchHost)
- description and source-code
```javascript
matchHost = function (host) {
  var match = (host || '').match(/([^\.]+)\.(?:([^\.]*)\.)?amazonaws\.com$/)
  var hostParts = (match || []).slice(1, 3)

  // ES's hostParts are sometimes the other way round, if the value that is expected
  // to be region equals ‘es’ switch them back
  // e.g. search-cluster-name-aaaa00aaaa0aaa0aaaaaaa0aaa.us-east-1.es.amazonaws.com
  if (hostParts[1] === 'es')
    hostParts = hostParts.reverse()

  return hostParts
}
```
- example usage
```shell
...
// request: { path | body, [host], [method], [headers], [service], [region] }
// credentials: { accessKeyId, secretAccessKey, [sessionToken] }
function RequestSigner(request, credentials) {

if (typeof request === 'string') request = url.parse(request)

var headers = request.headers = (request.headers || {}),
    hostParts = this.matchHost(request.hostname || request.host || headers.Host || headers.host)

this.request = request
this.credentials = credentials || this.defaultCredentials()

this.service = request.service || hostParts[0] || ''
this.region = request.region || hostParts[1] || 'us-east-1'
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.parsePath"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>parsePath ()](#apidoc.element.aws4.RequestSigner.prototype.parsePath)
- description and source-code
```javascript
parsePath = function () {
  var path = this.request.path || '/',
      queryIx = path.indexOf('?'),
      query = null

  if (queryIx >= 0) {
    query = querystring.parse(path.slice(queryIx + 1))
    path = path.slice(0, queryIx)
  }

  // S3 doesn't always encode characters > 127 correctly and
  // all services don't encode characters > 255 correctly
  // So if there are non-reserved chars (and it's not already all % encoded), just encode them all
  if (/[^0-9A-Za-z!'()*\-._~%/]/.test(path)) {
    path = path.split('/').map(function(piece) {
      return querystring.escape(querystring.unescape(piece))
    }).join('/')
  }

  this.parsedPath = {
    path: path,
    query: query,
  }
}
```
- example usage
```shell
...
  var region = this.isSingleRegion() ? '' :
    (this.service === 's3' && this.region !== 'us-east-1' ? '-' : '.') + this.region,
  service = this.service === 'ses' ? 'email' : this.service
  return service + region + '.amazonaws.com'
}

RequestSigner.prototype.prepareRequest = function() {
  this.parsePath()

  var request = this.request, headers = request.headers, query

  if (request.signQuery) {

this.parsedPath.query = query = this.parsedPath.query || {}
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.prepareRequest"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>prepareRequest ()](#apidoc.element.aws4.RequestSigner.prototype.prepareRequest)
- description and source-code
```javascript
prepareRequest = function () {
  this.parsePath()

  var request = this.request, headers = request.headers, query

  if (request.signQuery) {

    this.parsedPath.query = query = this.parsedPath.query || {}

    if (this.credentials.sessionToken)
      query['X-Amz-Security-Token'] = this.credentials.sessionToken

    if (this.service === 's3' && !query['X-Amz-Expires'])
      query['X-Amz-Expires'] = 86400

    if (query['X-Amz-Date'])
      this.datetime = query['X-Amz-Date']
    else
      query['X-Amz-Date'] = this.getDateTime()

    query['X-Amz-Algorithm'] = 'AWS4-HMAC-SHA256'
    query['X-Amz-Credential'] = this.credentials.accessKeyId + '/' + this.credentialString()
    query['X-Amz-SignedHeaders'] = this.signedHeaders()

  } else {

    if (!request.doNotModifyHeaders && !this.isCodeCommitGit) {
      if (request.body && !headers['Content-Type'] && !headers['content-type'])
        headers['Content-Type'] = 'application/x-www-form-urlencoded; charset=utf-8'

      if (request.body && !headers['Content-Length'] && !headers['content-length'])
        headers['Content-Length'] = Buffer.byteLength(request.body)

      if (this.credentials.sessionToken && !headers['X-Amz-Security-Token'] && !headers['x-amz-security-token'])
        headers['X-Amz-Security-Token'] = this.credentials.sessionToken

      if (this.service === 's3' && !headers['X-Amz-Content-Sha256'] && !headers['x-amz-content-sha256'])
        headers['X-Amz-Content-Sha256'] = hash(this.request.body || '', 'hex')

      if (headers['X-Amz-Date'] || headers['x-amz-date'])
        this.datetime = headers['X-Amz-Date'] || headers['x-amz-date']
      else
        headers['X-Amz-Date'] = this.getDateTime()
    }

    delete headers.Authorization
    delete headers.authorization
  }
}
```
- example usage
```shell
...

  delete headers.Authorization
  delete headers.authorization
}
}

RequestSigner.prototype.sign = function() {
if (!this.parsedPath) this.prepareRequest()

if (this.request.signQuery) {
  this.parsedPath.query['X-Amz-Signature'] = this.signature()
} else {
  this.request.headers.Authorization = this.authHeader()
}
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.sign"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>sign ()](#apidoc.element.aws4.RequestSigner.prototype.sign)
- description and source-code
```javascript
sign = function () {
  if (!this.parsedPath) this.prepareRequest()

  if (this.request.signQuery) {
    this.parsedPath.query['X-Amz-Signature'] = this.signature()
  } else {
    this.request.headers.Authorization = this.authHeader()
  }

  this.request.path = this.formatPath()

  return this.request
}
```
- example usage
```shell
...

// alternatively (as aws4 can infer the host):
opts = {service: 'sqs', region: 'us-east-1', path: '/?Action=ListQueues'}

// alternatively (as us-east-1 is default):
opts = {service: 'sqs', path: '/?Action=ListQueues'}

aws4.sign(opts) // assumes AWS credentials are available in process.env

console.log(opts)
/*
{
host: 'sqs.us-east-1.amazonaws.com',
path: '/?Action=ListQueues',
headers: {
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.signature"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>signature ()](#apidoc.element.aws4.RequestSigner.prototype.signature)
- description and source-code
```javascript
signature = function () {
  var date = this.getDate(),
      cacheKey = [this.credentials.secretAccessKey, date, this.region, this.service].join(),
      kDate, kRegion, kService, kCredentials = credentialsCache.get(cacheKey)
  if (!kCredentials) {
    kDate = hmac('AWS4' + this.credentials.secretAccessKey, date)
    kRegion = hmac(kDate, this.region)
    kService = hmac(kRegion, this.service)
    kCredentials = hmac(kService, 'aws4_request')
    credentialsCache.set(cacheKey, kCredentials)
  }
  return hmac(kCredentials, this.stringToSign(), 'hex')
}
```
- example usage
```shell
...
// Generate CodeCommit Git access password
var signer = new aws4.RequestSigner({
  service: 'codecommit',
  host: 'git-codecommit.us-east-1.amazonaws.com',
  method: 'GIT',
  path: '/v1/repos/MyAwesomeRepo',
})
var password = signer.getDateTime() + 'Z' + signer.signature()
'''

API
---

### aws4.sign(requestOptions, [credentials])
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.signedHeaders"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>signedHeaders ()](#apidoc.element.aws4.RequestSigner.prototype.signedHeaders)
- description and source-code
```javascript
signedHeaders = function () {
  return Object.keys(this.request.headers)
    .map(function(key) { return key.toLowerCase() })
    .sort()
    .join(';')
}
```
- example usage
```shell
...
if (query['X-Amz-Date'])
  this.datetime = query['X-Amz-Date']
else
  query['X-Amz-Date'] = this.getDateTime()

query['X-Amz-Algorithm'] = 'AWS4-HMAC-SHA256'
query['X-Amz-Credential'] = this.credentials.accessKeyId + '/' + this.credentialString()
query['X-Amz-SignedHeaders'] = this.signedHeaders()

  } else {

if (!request.doNotModifyHeaders && !this.isCodeCommitGit) {
  if (request.body && !headers['Content-Type'] && !headers['content-type'])
    headers['Content-Type'] = 'application/x-www-form-urlencoded; charset=utf-8'
...
```

#### <a name="apidoc.element.aws4.RequestSigner.prototype.stringToSign"></a>[function <span class="apidocSignatureSpan">aws4.RequestSigner.prototype.</span>stringToSign ()](#apidoc.element.aws4.RequestSigner.prototype.stringToSign)
- description and source-code
```javascript
stringToSign = function () {
  return [
    'AWS4-HMAC-SHA256',
    this.getDateTime(),
    this.credentialString(),
    hash(this.canonicalString(), 'hex'),
  ].join('\n')
}
```
- example usage
```shell
...
if (!kCredentials) {
  kDate = hmac('AWS4' + this.credentials.secretAccessKey, date)
  kRegion = hmac(kDate, this.region)
  kService = hmac(kRegion, this.service)
  kCredentials = hmac(kService, 'aws4_request')
  credentialsCache.set(cacheKey, kCredentials)
}
return hmac(kCredentials, this.stringToSign(), 'hex')
}

RequestSigner.prototype.stringToSign = function() {
return [
  'AWS4-HMAC-SHA256',
  this.getDateTime(),
  this.credentialString(),
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
