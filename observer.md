An admin can get a holistic view of the current and past health of their device in one place.

User stories:

    Any user can quickly toggle the "Bandwidth" and "Usage" tabs between their existing view and the Observer beta (BETA only)

    Any user can provide feedback on their experience in the Observer beta through via the Control portal (BETA only)

    Any user can access the blog post to learn more about our work on Observer inside the beta experience (BETA only)

    Users have one designated place where they can store and view infrastructure resource metrics for virtual servers:

    1. CPU utilization, %, per virtual core

    2. Network-Public, in/out, bytes and packets

    3. Network- Private, in/out, bytes and packets

    4. Memory utilization, %

    5. Disk Read, bytes and ops

    6. Disk Write, bytes and ops

    7. Transmit errors, in/out, count

    8. Disk Latency, ms, read and write

    9. Local disk utilization, % and bytes used and total bytes available


    Bare metal users will be able to view the following metrics:

    1. CPU utilization, %, per virtual core

    2. Network-Public, in/out, bytes and packets

    3. Network- Private, in/out, bytes and packets

    4. Memory utilization, %

    5. Disk Read, bytes and ops

    6. Disk Write, bytes and ops

    7. Transmit errors, in/out, count

    8. Disk Latency, ms, read and write

    9. Local disk utilization, % and bytes used and total bytes available

    10. RAID Alerts, 0/1

    11. Core temperature, degrees F

    Any admin can view history of alarms and metrics in a single view without having to do any logging analysis. (similar to #60)

    A manager can understand the general health of their device without needing clarification from their admin teams.

    Any user can open a device's most recent syslog file without using the command line (similar to #35)

    Any user can view and explore any time series metric data in a set of interactive charts.

    Any user can view and make basic sense of alert history.

    Any user can mark events as "open" or "closed".

    No users need to manually create an event whenever an alarm is triggered.

    No users need to manually assign a severity level of "warning" or "error" aside from their alarm settings.

    Any user can gather system and application level metrics using collectD agents for monitoring processes, apache, tomcat, MSSQL, MySQL, and URL responses.

    An admin can send custom metric data into the monitoring service in an automated way.

    Any user can utilize system, application, or custom metrics the same way as hypervisor metrics: graphs, dashboards, alarms, notifications, auto-responses, templates, etc.



Hill 2: An admin can understand and start to troubleshoot an incident within 90 seconds

User stories:

    Any admin can subscribe to alerts without being inundated with false positives.

    Any admin can receive alerts via their first choice communication channel within a minute of a triggering event.

    Reliability engineers can understand the cause of an incident alert based on the message in the alert itself.

    Any admin can check recent usage metrics on any device with a high degree of accuracy.

    Any admin can search for the exact information they need in under 10 seconds.

    A non-admin can resolve an escalated incident with fewer than three messages from SL support

    Any user can specify a condition to alert off of for any metric that is available (default, collectD, or custom).

    Any user can specify a condition based on average value, cumulative (sum) value, minimum value, or maximum value of any metric.

    Any user can specify a condition with the qualification "greater than" or "less than".

    Any user can specify the number of consecutive periods that a condition must be met, as well as the length of the period either 30 seconds or 5 minutes, before an alarm is triggered- "if X occurs for 2 consecutive periods of 30 seconds, then alarm is triggered"

    Any user can specify multiple conditions for a single alarm- "if this AND this AND this, then alarm triggered".

    Any user can specify a custom name for the alarm.

    Any user can be informed of alerts indicating the time, alarm name, and the conditions that were met that triggered the alarm.

    No users, after an alarm is triggered, will receive additional alerts from the same rule on the same device until the intial alarm has been "closed".

    Example alarm rule: If the average of CPU Utilization is greater than 80% for 2 consecutive periods of 5 minutes AND the sum of Network inbound is greater than 50 GBs for 1 consecutive period 5 minutes an alarm is triggered and an event is created (assuming any previous alarms from this rule have been closed)

    An admin can specify 1 or more email addresses to notify any user.

    An admin can specify 1 or more SMS phone numbers to notify any user.

    An admin can specify 1 or more URLs for webhooks to send.

    An admin can specify Pagerduty group to notify users.

    An admin can specify if the server should reboot or shut down when the alarm is triggered.

    An admin can specify an interval of 30 seconds or 5 minutes for network monitoring of any supported protocol

    An admin can implement host ping (ICMP) checks

    An admin can implement TCP port checks for various protocols: DNS, DNS custom, FTP, HTTP, HTTP custom, HTTPS, IMAP, LDAP, NNTP, POP, SMTP, SSH, TCP Custom, TELNET, UDP SIP (support for these protocols exist in current SL TCP offering)

    An admin can implement a TCP port check for the SNMP protocol (not currently supported in existing SL offering)

    An admin can specify threshold for the response time to qualify as a success or an error

    An admin can specify the number of consecutive errors from a host ping or TCP port check before an alarm is triggered.

    An admin can implement the same notification and automated response options from network monitoring alarms as from alarms based on metrics (email, SMS, webhook, PagerDuty, reboot, shutdown)

    An admin can specify severity level of "warning" or "error" for both metric and network monitoring alarms.



Hill 3: Any user can set up monitoring on any device, spending less than 90 seconds on configuration decisions. (similar to #59)

User stories:

    A non-admin can basically configure their monitoring using only the interface and documentation.

    An admin can set up monitoring that meets their specific needs by picking saved or pre-packaged configurations without going through the manual configuration process. (similar to #58)

    An admin can set up monitoring that meets their specific needs by manually editing and saving a configuration and apply it to any number of devices.

    An admin can set up alerts on multiple devices with minimal repetitive effort.

    Any user can export time- and metric-specific data in a CSV file.

    An admin or manager can set up a maintenance window during which time no notifications will be sent when alarms are triggered.

    Any established user can understand and apply saved configurations. (similar to #41)

    Any new user can understand and apply prepackaged configurations. (similar to #34, #32)

    A non-admin can get support on setting up monitoring without filing a support ticket.

    Any customer can order monitoring for any device without expert knowledge. (similar to #63, #43)

    All customers have a unified, predictable experience for ordering monitoring for any device. (similar to #40)

    Any user can integrate their device with a third party service without filing a support ticket.

    No users need to manually create an alarm for lifecycle "warning" alerts: creation, boot, shut down.

    Any technical user can access all Observer functionality through the same API as the rest of the monitoring service.

    IBM can restrict ab accounts access to certain features/performance with free version as defined in the Observer Overview for the free vs paid tier.

    Any customer can upgrade from free to paid version inside the monitoring tab.

    Any customer can upgrade or downgrade from paid or free versions in the account management area.

    Any user with the free version can view the options they would have if they upgraded, but in a way that indicates why they are unavailable

    If a user tries to perform an action that would require an upgrade to perform, they should see a message that explains they need to upgrade and offers an alternative if one exists (eg, "you already have the maximum number of alarms for the free version. upgrade or delete an alarm to create a new rule").


