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

## Tools For Sensitive data

1. Private data => bcrypt / crypto - https://www.npmjs.com/package/bcrypt
2. Code and functions => https://jscrambler.com/
3. Unsecured HTTP => HTTPS

## XML external entities

- XML External Entities have been promoted to a top 10 issue on OWASP and for a good reason. This attack occurs when an XML document is malformed and could be exploited for DOS attacks.
- In this scenario, the attacker exploited the XML malformed document that takes a bit more time to process due to its structure, and then leveraged this bad XML document to render the resource processing unit useless, therefore denying its users of the resource, which is a denial of service or DOS attack.
- If in your application you are using XML documents, make sure you're using proper syntax as you could be subjecting your users to not only slower performance, but also opening up an opportunity for a hacker to attack your systems with a DOS attack.

## Insufficient logging and monitoring

- Take this scenario, on average your website or application gets about 200 users per day. And you allocated resource for that workload. But, all of a sudden, your application jumps to 500 users, then 1,000 or more. How will you know about the sudden surge in users? How will you be able to react to it and even worse, how will you determine if this is an official user growth or a hacker sending his minions for a typical DOS attack?
- Monitoring and logging is key to supervisor resources, user growth, and yes, hackers on the prowl towards your application.
- Most host providers have a decent amount of tools you can use for this purpose.
- Set alerts so you get notifications for unusual behaviors.
- Make sure you set some type of user-based monitoring and you can either use pre-built resources such as Google Analytics, Elastic Search, or build your own within your application.
