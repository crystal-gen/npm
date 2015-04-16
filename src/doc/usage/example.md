```yaml
name: npm-test
version: 0.1.0

generators:
  npm:
    spec:
      private: true
      dependencies:
        - name: body-parser
          version: "~1.12.2"
        - name: cookie-parser
          version: "~1.3.4"
        - name: express
          version: "~4.12.2"
        - name: express-session
          version: "~1.10.4"
    version: latest
```