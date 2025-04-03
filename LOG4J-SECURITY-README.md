# Critical Log4j Security Update

    This file contains instructions needed to address critical Log4j vulnerabilities (CVE-2021-44228, CVE-2021-45046).

    ## Required Actions

    1. **Dependency Updates**: Add these dependencies to your project:
    - `org.apache.logging.log4j:log4j-core:2.17.1`
    - `org.apache.logging.log4j:log4j-api:2.17.1`

    2. **Configuration**: Add to application.properties:
    - `log4j2.formatMsgNoLookups=true`

    3. **Force Resolution**: Add explicit version resolution to override transitive dependencies

    **IMPORTANT**: This is a critical security update. These vulnerabilities allow remote code execution.
    