# mac-fc-scan-github-releases

This (public) repo is used to store releases of the `scan-github` CLI from the [mac-fc-dso-metrics repo](https://github.com/Enterprise-CMCS/mac-fc-dso-metrics). We do this because:
- we want the `scan-github` GitHub Action from the [mac-fc-report-dso-event repo](https://github.com/Enterprise-CMCS/mac-fc-report-dso-event) to be able to list and download release binaries using the default `GITHUB_TOKEN` granted to Actions workflows
- the `GITHUB_TOKEN` can list releases for public repos but not internal ones
- the [mac-fc-dso-metrics repo](https://github.com/Enterprise-CMCS/mac-fc-dso-metrics) is internal, and we want to keep it that way

So, this intermediate release repo allows our Action to consume these binaries without exposing the source code and other implementation details.
