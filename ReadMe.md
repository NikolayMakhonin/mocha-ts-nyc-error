# Reproduce the error

* OS: Windows 10
* NodeJS: v14.19.3

```
npm i
npm test
```

you should see this:
```
C:\projects\mocha-ts-nyc-error>npm test

> mocha-ts-nyc-error@1.0.0 test C:\projects\mocha-ts-nyc-error
> nyc --reporter lcov mocha -r ts-node/register ./src/qwe.test.ts



  test
OK
OK
    v test


  1 passing (7ms)

Path contains invalid characters: C:\projects\mocha-ts-nyc-error\coverage\lcov-report\1\file:\C:\projects\mocha-ts-nyc-error\src\1
 ELIFECYCLE  Test failed. See above for more details.
```
