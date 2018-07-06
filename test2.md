Lansweeper lets you send 2 types of asset alerts: alerts for reports listed in the web console's Reports tab, which are sent on a scheduled basis, and event log alerts, which are sent as soon as the Windows event log entries specified by you are scanned. Sending alerts is useful for tracking vital network information, software and other changes, server or workstation errors and more! Both report and event log alerts can be sent via email. From Lansweeper 6.0 onward, report alerts can be copied to a directory as well, instead of being sent via email.
<h2>Configuring email alerts</h2>
Report and event log alerts are configured in the <span style="background-color: #ffd1a4;">Configuration\Email Alerts</span> section of the web console. If you plan on having your alerts sent via email, be sure to, prior to configuring your actual alerts enter your SMTP server, port number, the email address you would like to send from and its display name into the correct input boxes. Optionally, you can load a built-in SMTP configuration, use SSL and/or enable authentication. There's also a button to test your SMTP settings.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-1.jpg" alt="SMTP configuration for report and event log alerts" />

Hit the <span style="background-color: #cdebf3;">Add E-mail Group</span> button. An email group is a collection of email addresses your alerts will be sent to. Enter a name for the group into the upper input box of the popup window. In the second input box, enter one or more email addresses, separated with semicolons. Then hit Ok. You can create multiple email groups to send various alerts to.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-2.jpg" alt="creating email groups for report and event log alerts" />
<h2>Setting up report alerts</h2>
To set up a report alert, tick the <span style="background-color: #cdebf3;">Enable report mailing</span> checkbox.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-3.jpg" alt="enabling report alerts" />
<h3>Step 1: Add a report</h3>
Hit the <span style="background-color: #cdebf3;">Add report</span> button, select one or more reports and hit <span style="background-color: #cdebf3;">Add</span>. You can use the search box to find specific reports.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-4.jpg" alt="selecting reports for report alerts" />
<div style="background: #ffffd5; padding: 15px; color: #262626;"><img src="https://www.lansweeper.com/wp-content/uploads/2018/06/lightbulb.png" alt="" /> A report is only mailed if it has results. Empty reports are not mailed.</div>
<h4></h4>
<h3>Step 2: Select an Alert and Export type</h3>
For each report, choose whether to have it sent via email or copied to a directory and choose an export type as well. Available export formats are Excel, CSV and HTML. If you choose Directory as your Alert Type, the report file is copied to the following folder on the machine hosting your Lansweeper installation: <span style="color: #e36c0b;">Program Files (x86)\Lansweeper\Service\export</span>

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-5.jpg" alt="choosing an alert type and export format for report alerts" />
<h3>Step 3: Set a time schedule</h3>
Hit the <span style="background-color: #cdebf3;">Set time schedules</span> button to select the schedule to be used for the report alert. The resulting popup lists a number of built-in schedules, but you can create your own as well, with the available button in the popup window.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-6.jpg" alt="choosing a schedule for report alerts" />
<h3>Step 4: Select an Email Group</h3>
If you chose E-mail as your Alert Type, choose an email group to send the report alert to.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-7.jpg" alt="choosing an email group for report alerts" />

If you chose Directory as your Alert Type, optionally tick the Overwrite checkbox. If this box is checked, a report's results will be overwritten in the export folder every time the alert is triggered. If this box is unchecked, a new file will be generated in the export folder every time the alert is triggered.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-8.jpg" alt="overwrite option for report alerts" />

The reports will now be sent based on the schedules specified by you. You can immediately have all reports mailed as well by hitting the <span style="background-color: #cdebf3;">E-mail /  save all configured reports now</span> button.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-9.jpg" alt="report alert sent via email" />
<h2>Setting up event log alerts</h2>
To set up an event log alert tick the <span style="background-color: #cdebf3;">Enable eventlog alerts</span> checkbox.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-10.jpg" alt="enabling event log alerts" />
<h3>Step 1: Add an event</h3>
Hit the <span style="background-color: #cdebf3;">Add event filter</span> button, select an event from the list of scanned events and hit Ok. Alternatively, you can manually type an event source and event ID in the popup window, if you would like to create an alert for an event that hasn't been scanned yet.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-11.jpg" alt="choosing an event for event log alerts" />
<div style="background: #ffffd5; padding: 15px; color: #262626;"><img src="https://www.lansweeper.com/wp-content/uploads/2018/06/lightbulb.png" alt="" /> Keep in mind that, to keep your database as small as possible, only error events are scanned by default. To generate alerts for non-error events, make sure <a href="http://www.lansweeper.com/kb/128/scanning-non-error-events.html" target="_blank" rel="noopener">the necessary event types are enabled</a> for scanning.</div>
<h4></h4>
<h3>Step 2: Customize your criteria</h3>
You can modify the criteria the event has to meet to generate an alert. Hit the pencil shaped edit button next to the event and then <span style="background-color: #cdebf3;">Add Filter</span> in the resulting popup.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-12.jpg" alt="modifying the criteria of an event log alert" />
<ul>
 	<li><strong>Computer</strong>: NetBIOS name of the computer generating the event.</li>
 	<li><strong>Domain</strong>: (NetBIOS) name of the domain/workgroup the event originates from.</li>
 	<li><strong>EventID</strong>: numeric code identifying the event.</li>
 	<li><strong>Eventtype</strong>: Error, Warning, Information, FailureAudit or SuccessAudit.</li>
 	<li><strong>Logfile</strong>: specific log the event belongs to.</li>
 	<li><strong>Source</strong>: source of the event.</li>
 	<li><strong>User</strong>: user that was logged into the computer when the event was generated.</li>
 	<li><strong>Message</strong>: comment included in the event.</li>
</ul>
<div style="background: #ffffd5; padding: 15px; color: #262626;"><img src="https://www.lansweeper.com/wp-content/uploads/2018/06/lightbulb.png" alt="" /> You can use the Like/Not Like operators and the % sign to look for partial matches.
• "Computer Like LAN%" means: any computer whose name starts with the word “LAN”.
• "Computer Like %LAN" means: any computer whose name ends in the word “LAN".
• "Computer Like %LAN%" means: any computer whose name contains the word “LAN”.</div>
<h4></h4>
<h3>Step 3: Select an email group</h3>
For each event, select the email group you want to send the alerts to.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-13.jpg" alt="choosing an email group for event log alerts" />

As soon as the specified event is scanned, an email is sent to the mail group of your choice.

<img class="aligncenter" style="border: 1px dotted black;" src="https://www.lansweeper.com/wp-content/uploads/2018/06/sending-report-and-event-log-alerts-14.jpg" alt="event log alert sent via email" />
<div style="background: #ffffd5; padding: 15px; color: #262626;"><img src="https://www.lansweeper.com/wp-content/uploads/2018/06/lightbulb.png" alt="" /> Event alerts are best used in combination with <a href="http://www.lansweeper.com/kb/127/scanning-with-scheduled-eventlog-scanning.html" target="_blank" rel="noopener">Eventlog Only scanning targets</a>. Eventlog Only scanning targets allow you to scan event log entries as frequently as once a minute, ensuring that you receive your email alerts near-instantaneously.</div>
