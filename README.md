# Serverless template for Aws, Nodejs & ReasonML

Make sure you have the [bucklescript compiler](https://bucklescript.github.io/)
installed:

```
npm install -g bs-platform
```

Now build your project:

```
npm run build       # To build once
npm run build:watch # To build indefinitely
```

This builds all of the reason files into js files alongside the originals. If
you ever want to clean out the compiled files you should run:

```
npm run clean
```

Once you have built your project, test that it all works as expected:

```
serverless invoke local -f hello
```

Which should print out:

```
"Hello world!"
```

Now have a look in `src/Hello.re` and get started on your project!