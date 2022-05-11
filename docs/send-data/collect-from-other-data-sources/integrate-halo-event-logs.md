---
id: integrate-halo-event-logs
---

# Integrate Halo Event Logs into Sumo Logic

The Halo Event Connector enables you to pull security event logs from Halo into Sumo Logic, including alerts from your configuration, file integrity, and software vulnerability scans. Halo can also deliver unprecedented visibility of your cloud servers, directly into your log management console. You can track server events such as your server rebooting, shutting down, changing IP addresses, and much more.

Using the scripts and documentation posted on Github https://github.com/cloudpassage/halo-event-connector-python,
you can quickly and easily set up a Source so events generated by Halo will feed into your log management system, giving you centralized, and more complete visibility across your server environment.

The Halo Event Connector is free to use, and will work with any Halo subscription.  

**To integrate Halo events into Sumo Logic:**

1. Make sure you have set up accounts for [CloudPassage Halo](http://pages.cloudpassage.com/halo-pro.html) and Sumo Logic.
1. [Generate an API key](https://support.cloudpassage.com/entries/23631996-Generating-an-API-key) in your CloudPassage Halo portal.  
1. Once you have an API key, follow the steps provided in the [Sumo Logic - Halo Documentation](https://github.com/cloudpassage/halo-event-connector-python/blob/master/Halo-Event-Connector_SumoLogic.pdf), using the files provided on Github https://github.com/cloudpassage/halo-event-connector-python.

The documentation available with those files on GitHub walks you through the process of testing the Halo Event Connector script.  
