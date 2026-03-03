## 🚀 Major Features
### Performance Improvements => Automatic Data Cleanup ([MST-986](https://bhp1.atlassian.net/browse/MST-986))
* Implemented automatic cleanup of out-of-scope data when cloning scenarios into new periods
* Improved resource group configuration and document path strategies

### Performance Improvements => Automated Git Repository maintenance ([MST-1033](https://bhp1.atlassian.net/browse/MST-1033))
* Implemented cron job for automated Git repository maintenance
* Improved repository management and cleanup processes

### Improved Scenario Creation UX ([MST-996](https://bhp1.atlassian.net/browse/MST-996))
* Improved layout and user experience for creating new scenarios
* Enhanced scenario creation flow with modal dialog instead of inline form

## 🐛 Bug Fixes
### Connected Excel File Download ([MST-983](https://bhp1.atlassian.net/browse/MST-983))
* Fixed ApiUrlBase for connected Excel spreadsheet downloads
* Added Excel template paths for staging and production with correct Linux path delimiters
* Removed references to decommissioned servers

### Unit Test Stability ([MST-1034](https://bhp1.atlassian.net/browse/MST-1034))
* Fixed intermittent test failures in Azure DevOps
* Added cancellation token support for background tasks in Repository.cs
* Enhanced test teardown procedures with proper GC collection and cleanup timing
* Implemented consistent cleanup patterns across all test files

### Kubernetes Ingress Configuration
* Fixed pathType in ingress template to conform with updated validation rules
* Resolved silent Helm upgrade failures

## 🔧 Maintenance & Upgrades
### Angular v15 Upgrade ([MST-1031](https://bhp1.atlassian.net/browse/MST-1031))
* Upgraded Angular framework from v14 to v15. This is a pre-requirement to improving Authentication experience
* Removed unused references to Keycloak
* Improved build time by 30 seconds

### Performance Monitoring & Telemetry ([MST-1012](https://bhp1.atlassian.net/browse/MST-1012))
* Integrated Azure Application Insights for performance tracking
* Added telemetry for publication and clone-and-change workflows
* Performance metrics now tracked for save operations