# Gradle + Spring Boot Example

This example shows how to use Gradle with Spring Boot.

Please read [Get Groovy with Gradle](https://developer.okta.com/blog/2019/09/03/gradle-tutorial) to learn more.

**Prerequisites:** [Java 8](https://adoptopenjdk.net)

> [Okta](https://developer.okta.com/) has Authentication and User Management APIs that reduce development time with instant-on, scalable user infrastructure. Okta's intuitive API and expert support make it easy for developers to authenticate, manage and secure users and roles in any application.

* [Getting Started](#getting-started)
* [Help](#help)
* [Links](#links)
* [License](#license)

## Getting Started

To install this example application, run the following commands:

```bash
git clone https://github.com/oktadeveloper/okta-spring-boot-gradle-example.git
```

This will get a copy of the project locally. 

### Create an OIDC App in Okta

Log in to your Okta Developer account (or [sign up](https://developer.okta.com/signup/) if you don’t have an account) and navigate to **Security** > **API**. Grab the issuer value from your `default` authorization server.

Copy it into `gradle.properties`:

```properties
oauthIssuer=https://{yourOktaDomain}/oauth2/default  
```

**NOTE:** The value of `{yourOktaDomain}` should be something like `dev-123456.okta.com`. Make sure you don't include `-admin` in the value!

### Start the application

To start the application you can just run:

```bash
./gradlew bootRun
```

## Links

This example uses the [Okta Spring Boot Starter](https://github.com/okta/okta-spring-boot) to integrate with Okta.

## Help

Please post any questions as comments on the following blog posts, or visit our [Okta Developer Forums](https://devforum.okta.com/).

## License

Apache 2.0, see [LICENSE](LICENSE).
