# Server-Side Exploits

## Server Side Attack Vectors
* Lack of encryption (plain text passwords)
* Broken authentication workflows
* Session info not expiring or exposing user info
* SQL Injection
* Cross Site Request Forgery

> Never log or print the user's password anywhere.

![password](img/password.jpg)

As a Make School student, we know you'd _never_ store sensitive information without using some kind of security. But companies like [Facebook/Instagram](https://newsroom.fb.com/news/2019/03/keeping-passwords-secure/) and [Google](https://cloud.google.com/blog/products/g-suite/notifying-administrators-about-unhashed-password-storage) have _RECENTLY_ experienced these issues!

#### How to Avoid This

- Use SSL
  - **Developers**: Use [Let's Encrypt](https://letsencrypt.org/) to generate free SSL certificates for your deployments.
  - **End Users**: Check out the [HTTPS Everywhere](https://www.eff.org/https-everywhere) extension for your browser to constantly reinforce this!
- **Encrypt credentials** on the server
  - Use [bcrypt](https://github.com/Make-School-Courses/BEW-2.3-Web-Security/tree/master/Lessons) with high entropy!
