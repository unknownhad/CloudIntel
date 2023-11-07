# IOC Consumption Guide for AWS Infrastructure

This guide details how to consume the IP-based Indicators of Compromise (IOCs) that have been observed attacking AWS infrastructure.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Understanding the IOCs](#understanding-the-iocs)
- [Integrating IOCs with AWS Services](#integrating-iocs-with-aws-services)
- [Automating IOC Updates](#automating-ioc-updates)
- [Contact and Support](#contact-and-support)

## Introduction

The IOCs provided in this repository consist of IP addresses that have been identified as sources of malicious activity against AWS services. They can be used to detect potential threats and enhance security measures.

## Prerequisites

- Active AWS account with appropriate permissions.
- Understanding of AWS security services and features.
- Familiarity with network security and incident response concepts.

## Understanding the IOCs

The IOCs are structured by date and contain lists of IP addresses. Each IP is provided with context on the nature of the observed attack where available.

## Integrating IOCs with AWS Services

You can use these IP-based IOCs with services such as AWS WAF, Amazon GuardDuty, or VPC Flow Logs for monitoring and protection.

### Step-by-Step Integration

1. **Select AWS Service**: Choose an AWS service that supports IP-based monitoring or blocking.
2. **Import IOCs**: Upload the list of malicious IPs to the service, following the specific guidelines provided by AWS for that service.
3. **Configure Monitoring or Blocking**: Set the service to alert you when traffic is detected from these IPs or to block them outright.
4. **Respond to Incidents**: Establish a response plan for alerts generated due to IOC detection.

## Automating IOC Updates

To maintain up-to-date security, automate the import of new IOCs:

- **AWS Lambda**: Use Lambda to periodically check the repository for updated IOC lists and import them into your chosen AWS service.
- **CloudWatch Events**: Trigger your Lambda function in response to scheduled events to refresh the IOCs.

## Contact and Support

For questions or assistance with these IOCs, please open an issue in the GitHub repository or contact via [me[at]himanshuanand.com](mailto:me@himanshuanand.com).

