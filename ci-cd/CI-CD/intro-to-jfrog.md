# What IS JFrog Artifactory?

## The General Components of JFrog 

## JFrog Xray CVE Scanning
<p>Complexities aside, JFrog also comes with an extensible feature that permits for artifact scanning of CVEs (Common Vulnerabilities and Exposures). The general workflow is stipulated below:</p>

<p>
    <ol>
        <li>A new application artifact is pushed onto the JFrog Artifactory.</li>
        <li>JFrog Xray scan is configured, subsequently triggering a CVE scan.</li>
    </ol>
</p>

<p>One of the major benefits of using JFrog is that through the command-line interface, it permits a trigger of the scan execution on demand. In my specific case, the CI/CD automation platform used is Atlassian Bamboo. The CLI is integrated with Bamboo via a plug-in, thus allowing the user to run CLI commands as Bamboo tasks. This also provides an added benefit, where developers can run their plans first, examine the CVE report and then decide if there is something that requires immediate remediation.</p>

<p>JFrog comes equipped with an independent database of CVEs. CVEs - or, common vulnerabilities and exposures - is defined as a dictionary of common names for publicly known InfoSec vulnerabilities. While the list is extensive, there have been a few noted to be historically and widely exploited, such as Log4Shell and EternalBlue.</p>

<p>When you view the JFrog log, you should see different status types.</p>

| Status Name | Explanation | 
|---|---|
| Not Scanned |---|
| Not Applicable |---|
| Not Covered |---|
| Applicable |---|
| Undetermined |---|

## How Do You Approach Resolving a CVE?
Section in progress.

## References

<ol>
    <li>https://en.wikipedia.org/wiki/Common_Vulnerabilities_and_Exposures</li>
    <li>https://jfrog.com/help/r/jfrog-security-user-guide/products/advanced-security/features-and-capabilities/contextual-analysis-of-cves</li>
    <li>https://en.wikipedia.org/wiki/EternalBlue</li>
    <li>https://en.wikipedia.org/wiki/Log4Shell</li>
    <li>https://www.reddit.com/r/cybersecurity/comments/123zkdo/how_do_you_deal_with_cve/</li>
</ol>