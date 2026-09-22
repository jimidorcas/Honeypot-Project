
# Honeypot Project

A hands-on cybersecurity project focused on deploying a honeypot, capturing malicious activity, and analysing real-world attack behaviour.

The project was designed to simulate an exposed system and observe how attackers interact with it, providing practical experience with **threat detection, log analysis, SSH security, network activity, and incident investigation**.

## Project Overview

The honeypot was deployed as an intentionally exposed environment designed to attract unauthorised connection attempts.

Captured activity was analysed to identify:

* Source IP addresses
* Connection and authentication attempts
* Successful and failed interactions
* Attack frequency
* Potential brute-force behaviour
* Common attacker activity
* Indicators that could support further investigation

The objective was not simply to collect logs, but to turn raw security events into meaningful observations about attacker behaviour.

## Key Findings

During the analysis, the honeypot captured **256 events from 45 unique IP addresses**.

Notable observations included:

* **45 unique source IP addresses**
* **256 total events**
* **6 successful logins**
* The most active IP generated **29 events**
* The second most active IP generated **23 events**

These results demonstrate how quickly an exposed service can attract unsolicited activity from multiple external sources.

> Note: A successful login recorded by the honeypot represents activity observed within the honeypot environment and should not automatically be interpreted as successful access to a real production system.

## Technologies & Tools

* Linux
* SSH
* Python
* Git & GitHub
* Log analysis
* IP address analysis
* Honeypot technology
* Command-line tools
* JSON/log data

## Skills Demonstrated

### Threat Detection

Identified suspicious connection and authentication activity from external IP addresses.

### Log Analysis

Analysed structured event data to identify patterns, frequency, and high-activity sources.

### Incident Investigation

Used captured evidence to investigate potentially malicious behaviour rather than relying solely on assumptions.

### Network Security

Explored how exposed services can become targets for automated scanning, probing, and unauthorised access attempts.

### Security Monitoring

Practised turning large volumes of security events into actionable information.

### Technical Documentation

Documented the deployment, observations, findings, and analysis in a reproducible format.

## Example Analysis

A simplified view of the captured activity:

| Metric                |        Result |
| --------------------- | ------------: |
| Total Events          |           256 |
| Unique IP Addresses   |            45 |
| Login Attempts        |             0 |
| Successful Logins     |             6 |
| Top Source IP         | 120.79.207.19 |
| Events from Top IP    |            29 |
| Second Most Active IP | 36.94.123.203 |
| Events from Second IP |            23 |

## Security Takeaways

This project reinforced several important security principles:

1. **Internet-facing services are continuously exposed to unsolicited activity.**
2. **Source IP analysis can help identify unusual or high-volume activity.**
3. **Logs provide valuable evidence for security investigations.**
4. **Authentication events should be monitored and investigated.**
5. **Security monitoring is most useful when raw events are converted into patterns and context.**
6. **A single event rarely tells the whole story; behaviour over time provides stronger investigative context.**

## Project Structure

```text
Honeypot-Project/
│
├── README.md
├── cowrie dashboard
└── virustotal scan
```

Additional project files contain the honeypot configuration, captured data, analysis, and supporting scripts.

## Future Improvements

Potential extensions to the project include:

* Automated IP reputation enrichment
* Geo-location analysis
* Attack-type classification
* Visual dashboards
* Automated alerting
* Integration with a SIEM
* MITRE ATT&CK technique mapping
* Detection rules for recurring attack patterns
* Automated reporting of high-risk activity

## What I Learned

This project provided practical experience in moving from **raw security telemetry to investigation and interpretation**.

Rather than treating every connection as an isolated event, the analysis focused on identifying patterns across source IPs, event frequency, authentication activity, and attacker behaviour.

This is the type of workflow used in security monitoring environments: **collect → detect → investigate → analyse → document**.

## Author

**Dorcas Olujimi**

Cybersecurity Analyst 

[GitHub](https://github.com/jimidorcas)

