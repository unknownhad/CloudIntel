# AWS Attacks Monitoring Project

This repository hosts resources and findings from a project aimed at monitoring attacks on AWS infrastructure, particularly focusing on cloud-native and cloud-only threats.

## Features
- Real-time data on malicious IP addresses, updated every 24 hours.
- (Under development) Malicious file detection API.
- Ongoing publication of data on GitHub.
  
## Consuming IOCs from this Repository

This repository is structured to aid in the monitoring of AWS infrastructure attacks, with a focus on cloud-native and cloud-only threats. It includes:

- Indicators of Compromise (IOCs)
- Malware Analysis
- Malware Samples

## Usage
To use the AWSAttacks API, make requests as follows:

```
curl -X GET
'https://cloudintel.himanshuanand.com/v1/maliciousip?date=MM-DD-YYYY'
-H 'x-api-key: [Your_API_Key]'
-H 'x-email: [Your_Email]'
```

Response format: JSON containing all observed malicious IP addresses.


### How to Use this Repository

1. **Understanding the Repository Structure**: Each folder is named with a date (DD-MM-YYYY) and contains daily collected IOCs.
2. **Reviewing Usage Warning**: Before using these IOCs, be aware of the risks. Executing code without understanding could be harmful.
3. **Accessing Malware Analysis**: For insights into the malware samples and their analysis, refer to the corresponding dated folders.
4. **Consuming IOCs**: Detailed instructions on how to consume these IOCs in your security operations will be provided in the [IOC Consumption Guide](IOC_CONSUMPTION.md). This guide will offer step-by-step instructions on how to integrate, automate, and utilize these IOCs with AWS services.
5. **Contributing**: If you have updates or additional IOCs, see the [Contribution Guidelines](CONTRIBUTING.md).
6. **Getting Support**: For questions or support, open an issue or reach out to [me[at]himanshuanand.com](mailto:me@himanshuanand.com).

## Documentation
For full details, visit our [Wiki](https://github.com/unknownhad/AWSAttacks/wiki/Welcome-to-the-AWSAttacks-Wiki!).

## Feature Requests and Contributions
For feature requests or contributions, open an [issue](https://github.com/unknownhad/AWSAttacks/issues).

## Acknowledgements
Special thanks to [Michel Bamps](https://github.com/michelbamps) for his expertise and assistance in integrating Cloudflare Workers with R2, a crucial part of the AWSAttacks infrastructure.

Remember to use the IOCs within the bounds of the [MIT License](LICENSE) and understand that this is a personal project, not associated with any employer.

For deeper insights into the project's purpose and methodology, refer to the accompanying [blog post]([blog.himanshuanand.com](https://blog.himanshuanand.com/posts/announcingawsattacks/)).
