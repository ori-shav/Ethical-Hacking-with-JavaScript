# Ethical-Hacking-with-JavaScript

Ethical Hacking with JavaScript Course - https://www.linkedin.com/learning/ethical-hacking-with-javascript/

## Tools to scan your code

1. `npm audit` - The audit command submits a description of the dependencies configured in your project to your default
   registry and asks for a report of known vulnerabilities. If any vulnerabilities are found, then the impact and appropriate
   remediation will be calculated. If the fixed argument the ithe s provided, then remediations will be applied to the package tree.
   https://docs.npmjs.com/cli/v8/commands/npm-audit

2. Snyk - Snyk (pronounced sneak) is a developer security platform for securing code, dependencies, containers,
   and infrastructure as code. sign up with GitHub and connect it to say then add the project to your project panel.
   once you have the report you can open a fix PR from snyk panel.
   https://snyk.io/

3. AppSensor - Real-time event detection, analysis and response. http://www.appsensor.org/getting-started.html

4. Retire.js - There are a plethora of JavaScript libraries for use on the web and in node.js apps out there.
   This greatly simplifies, but we need to stay updated on security fixes. "Using Components with Known Vulnerabilities" is
   now a part of the OWASP Top 10 and insecure libraries can pose a huge risk for your web app. The goal of Retire.js is to
   help you detect use of versions with known vulnerabilities.
   Retire.js has these parts:

- command line scanner -
- grunt plugin
- Chrome extension
- Firefox extension
- Burp and OWASP Zap plugin

```
$ npm install -g retire
$ retire
```

https://retirejs.github.io/retire.js/
