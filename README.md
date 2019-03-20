# text file crawler (tfc)

To quench my curiousity, I wanted to gauge the usage & adoption of the following
pseudo-standard text files:

- [`/robots.txt`][robots]
- [`/humans.txt`][humans]
- [`/.well-known/security.txt`][security]

Given a [`domains.txt`](/domains.txt) file containing one domain per line, the
Node.js script will fire off requests for each of the files. Given network I/O
is the constraint, this can take a while. There are basic checks for valid files
and redirects are followed to a degree. After completing, the statistics will be
printed out.

## Usage

```
npm install && npm start
```

## Thanks

[David][david].


[robots]: http://www.robotstxt.org/
[humans]: http://humanstxt.org/
[security]: https://securitytxt.org/
[david]: https://github.com/davidmerfield
