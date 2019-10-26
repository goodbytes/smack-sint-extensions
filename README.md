# smack-sint-extensions
Additional tests that add to those in [Smack's Integration Test Framework](https://github.com/igniterealtime/Smack/blob/master/documentation/developer/integrationtest.md).

# Run tests
To run tests, follow the instructions as provided in [Smack's Integration Test Framework](https://github.com/igniterealtime/Smack/blob/master/documentation/developer/integrationtest.md).

This is an example Run/Debug configuration (which you can use in Intellij):

- *Main class*: `org.igniterealtime.smack.inttest.SmackIntegrationTestFramework`
- *VM options*: `-Dsinttest.service=laptop-guus -Dsinttest.adminAccountUsername=admin -Dsinttest.adminAccountPassword=admin -Dsinttest.securityMode=disabled -Dsinttest.enabledTests=PubSubIntegrationTest`

Running a configuration like this will make the PubSubIntegrationTest tests run against an XMPP server running on the XMPP domain 'laptop-guus', using an administrator account that has as username/password: admin/admin.

This is the most basic configuration that you can use to run tests against a locally installed Openfire server. Obviously, change `laptop-guus` for the hostname of your laptop!
