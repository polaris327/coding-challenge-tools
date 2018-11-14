Coding Challenge Guidelines
===========================

Please organize, design, test, document your code as if it were
going into production, then send us a link to the hosted repository (e.g.
Github, Bitbucket...).

Functional spec
---------------

Prototype **one** of the following projects that is most suitable:

1. CRUD application - Front-end
2. Email Service - Back-end

### CRUD application - Front-end

Create React application with simple CRUD functionality for contracts. Contract data structure: 
``` js
{
   user: {
      name:string,
      surname: string
   },
   amountInUsd: string,
   currency: string,
   date: string  
}
```

You can create a simple express/koa server or use json-server to mock api. https://github.com/typicode/json-server 

**extra requirements:**
 * Display created contracts list in a table view. 
 * Add chart(s) using currency exchange rates: you can use ETH/USD exchange from https://www.coinapi.io/ (d3.js, chart.js or any other of your choice) 

The UX/UI is totally up to you. If you like, get creative and add additional
features a user might find useful!

You get some extra points for using TypeScript.

### Email Service - Back-end

Create a service that accepts the necessary information and schedules and sends emails in the future. 
It should be able to accept an arbitrary timestamp as an input for the email to be scheduled.
It should provide an abstraction between two different email service providers.
If one of the services goes down, your service can quickly failover to
a different provider without affecting your customers.

Example Email Providers:

* [SendGrid](https://sendgrid.com/user/signup) - [Simple Send Documentation](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
* [Mailgun](http://www.mailgun.com) - [Simple Send Documentation](http://documentation.mailgun.com/quickstart.html#sending-messages)
* [SparkPost](https://www.sparkpost.com/) - [Developer Hub](https://developers.sparkpost.com/)
* [Amazon SES](http://aws.amazon.com/ses/) - [Simple Send Documentation](http://docs.aws.amazon.com/ses/latest/APIReference/API_SendEmail.html)

All listed services are free to try and are pretty painless to sign up for, so
please register your own test accounts on each.

Technical spec
--------------

The architecture will be split between a back-end and a web front-end, for
instance providing a JSON in/out RESTful API. Feel free to use any other
technologies provided that the general client/service architecture is
respected.

Choose **one** of the following technical tracks that best suits your skillset:

1. **Full-stack**: include both front-end and back-end.
2. **Back-end track**: include a minimal front-end (e.g. a static view or API
   docs). Write, document and test your API as if it will be used by other
   services.
3. **Front-end track**: include a minimal back-end, or use json-server.
Focus on making the interface as polished as possible.

### Back-end

We believe there is no one-size-fits-all technology. Good engineering is about
using the right tool for the right job, and constantly learning about them.
Therefore, feel free to mention in your `README` how much experience you have
with the technical stack you choose, we will take note of that when reviewing
your challenge.

Here are some technologies we are more familiar with:

* Python
* JavaScript
* Go
* C++
* Rust
* Elixir
* Haskell
* Java

You are also free to use any web framework. If you choose to use a framework
that results in boilerplate code in the repository, please detail in your
README which code was written by you (as opposed to generated code).

### Front-end

The front-end app build should ideally be a single `index.html`
linking to external JS/CSS/etc and assets.


How will we review?
-------------------

[Guidelines can be found here](https://github.com/uber/coding-challenge-tools/blob/master/README.md)
