---
title: "Projects"
---

- [GCP Service Observer](https://github.com/jdyke/gcp_service_observer): This is an application that displays GCP Service/API endpoint information for a given GCP project ID. The frontend currently supports filtering and sorting. I created this to practice frontend coding but also to display a proof of concept on how this can be used for a better GCP API endpoint experience. This is not a production grade application so please do not use in your company's GCP environment.

- [GCP IAM Analyzer](https://github.com/jdyke/gcp-iam-analyzer): This is a command line IAM tool written in python to analyze GCP IAM roles and permissions. You can find the difference in 2 roles permissions, which permissions 2 roles share, list current permissions for a role, or find which role(s) have n + 1 permissions. All of this is done locally with no GCP permissions required.

- [GCP IAM monitor bot](https://github.com/jdyke/gcp_iam_update_bot): A bot that monitors and tweets when GCP updates their IAM roles. Follow [@gcp_iam_monitor](https://twitter.com/gcp_iam_monitor) to stay up to date on GCP IAM roles and their permissions.

- [GCP workload identity federation](https://github.com/ScaleSec/gcp-workload-identity-federation): A pypi module to enable workload identity federation from AWS to GCP without the need for static credentials.

- [Project Lockdown](https://github.com/ScaleSec/project_lockdown): This is an automated remediation project I created to show how to configure an end to end remediation application in GCP.

- [GCP organization policy bot](https://github.com/ScaleSec/gcp_org_policy_notifier): Another GCP bot but this time it monitors when GCP releases, deletes (yes that happens), or edits GCP [organization policy constraints](https://cloud.google.com/resource-manager/docs/organization-policy/org-policy-constraints). Follow [@gcporgpolicybot](https://twitter.com/gcporgpolicybot) to stay up to date.

- [Salesforce AWS allowlister](https://github.com/salesforce/aws-allowlister): I was a co-contributor on this repository providing guidance and quality assurance testing. This repo automatically compiles an AWS Service Control Policy that ONLY allows AWS services that are compliant with your preferred compliance frameworks.

- [Terraform AWS Service Control Policy Suite](https://github.com/ScaleSec/terraform_aws_scp): This repo is a collection of security and compliance focused AWS Service Control Policies (SCPs) written in Hashicorp Terraform to be used in AWS Organizations.

- [GCP service account lister](https://github.com/ScaleSec/gcp_sa_lister): A custom python tool that crawls your GCP organization and returns service accounts that have not been used in the past 90 days. Google does not provide an easy single pane of glass view into these types of metrics across thousands of projects so I created something to fill that gap.

- [GCP API key inventory](https://github.com/ScaleSec/gcp_api_key_inventory): Another custom python tool to inventory, analyze, and report on your GCP API keys in an automated fashion.

- [GCP ETD automation functions](https://github.com/ScaleSec/gcp_threat_detection_auto_remediation): A proof of concept application to begin automating [Event Thread Detection](https://cloud.google.com/security-command-center/docs/concepts-event-threat-detection-overview) findings in the [Security Command Center](https://cloud.google.com/security-command-center/docs/concepts-security-command-center-overview).
