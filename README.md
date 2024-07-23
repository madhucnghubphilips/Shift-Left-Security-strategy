<!-- GIF -->
<img align="center" height="300" width="500" src="https://github.com/madhucnghubphilips/Open-Source-Components-Usage/blob/main/Resource/coder3.gif" />
<!-- Header Section -->
<h1 align="center"><font face="Arial">Shift-left security strategy </font></h1>

<h2 align="left"><font face="Arial"><span style="color:green">What Shift-left security strategy?</span></font></h2>

Before we delve into the Shift-Left Security strategy, let's first understand what DevSecOps is.
<!-- PNG -->
<img align="right"  src="https://github.com/madhucnghubphilips/Shift-Left-Security-strategy/blob/main/Resources/DevSecOps.png" />

**Dev+Sec+Ops**, **__As Shannon Lietz - founder at DevSecOps foundation - said:__**<br>
The purpose and intent of DevSecOps is to build on the mindset that “everyone is responsible for security” with the goal of safely distributing security decisions at speed and scale to those who hold the highest level of context without sacrificing the safety required.”

**Shift-left security strategy**<br>
<font face="Arial">As a simple definition, the shift-left security strategy is a way or solution to embedding security as a part of our development process and **_consider security from the inception steps of application or system design_**. In other words, **_security is responsible for everyone who works in the software development and operating process._** Of course, security is a profession and we need highly skilled people to play security-related roles; but in this approach, any designer, software architecture, developer, DevOps engineer, and together with security guys have liability about security.</span></font>

<a href="https://owasp.org/www-project-devsecops-guideline/latest/00a-Overview">Reference: OWASP</a>


# Shift-left security strategy
The concept of "leftshift" in DevSecOps emphasizes integrating security early (shift-left) in the development lifecycle. This model focuses on embedding security practices from the very beginning of the development process.


<table>
	<tr>
		<td><h4>Maturity Level</h4></td> 
		<td><h4>Training</h4></td>
		<td><h4>Design Assessment</h4></td>
		<td><h4>Secure Code Review</h4></td>
		<td><h4>Security Testing</h4></td>
	</tr>
	<tr>
		<td>Stage 1:</td> 
		<td>Basic Security Training.</br>Provide initial security awareness training to development and operations teams.</br>Introduce fundamental security concepts and common vulnerabilities.</td>
		<td>Permissions</td>
		<td>As per tech stack, identify Basic SAST tools (Source code analysis tool, Open Source Software/code tool).</br>
Source code analysis tools: Fortify, Coverity, Checkmarx, Veracode, Bandit, Cppcheck.</br>
Open Source Software tools: BlackDuck, Snyk, WhiteSource, OWASP Dependency-Check, Retire.js, Clair.</br>
Introduce developers to SAST tools and their benefits.</br>
Provide basic training on how to use SAST tools effectively.</br></td>
		<td>Limitations</td>
	</tr>
	<tr>
		<td>Stage 2:</td> 
		<td>Establish security requirements and policies.</br>Document these requirements and ensure they are accessible to all teams.</br>**Guideline Documents:**</br>Input Parameter Validation Guidelines</br>Security Coding Guidelines</br>Sensitive Data Discovery Guidance for Development Teams</br>API/Web/Mobile/Thick Client/Hardware Security and Privacy Guidelines</td>
		<td>Permissions</td>
		<td>Select and implement a SAST tool that fits the organization’s technology stack and needs.</br>
On top of basic SASt tools, identify Sensitive information disclosure tool, IaC tool and Malware scan tools.</br>
Sensitive information disclosure tools: GitLeaks, TruffleHog, git-secrets.</br>
IaC tools: Checkov, Aqua Security, kics (Keeping Infrastructure as Code Secure), Pulumi.</br>
Malware scan tools: Malwarebytes, Bitdefender, Norton, McAfee.</br></td>
		<td>Limitations</td>
	</tr>
	<tr>
		<td>Stage 3:</td> 
		<td>Provide ongoing security training to keep the teams updated on the latest threats and best practices.</br>Encourage developers to take ownership of security by creating a security champions program.</br>**Introducing Tainings/Work Instructions.**</br>Security and Privacy Risk Management Procedure.</br>Security and Privacy Risk Management SAST Work Instructions.</br>Security and Privacy Risk Management DAST Work Instructions.</br>Security and Privacy Test Cases Procedure.</br>Cryptography and Key Management Standard</td>
		<td>Permissions</td>
		<td>Integrate SAST tools into the CI/CD pipeline to ensure that security scans are performed automatically with every build.</br></br>
Set up automated notifications for vulnerabilities detected during SAST scans.</br></td>
		<td>Limitations</td>
	</tr>
	<tr>
		<td>Stage 4:</td> 
		<td>Security & Privacy touch point sessions.</br>Involving in Release design and planning stage and overlook SAST status and CI-CD pipe lines</br>Insider Threat Mitigation Program Procedure</br>Open Source Software Vulnerability Management Procedure</td>
		<td>Permissions</td>
		<td>Ensure that all code, including third-party libraries and open-source components, is scanned by SAST tools.</br>
Regularly update SAST tools and their rule sets to cover the latest vulnerabilities.</br>
Develop necessary SAST gated builds.</br>
Promote the role of security champions within development teams who advocate for secure coding practices.</br></td>
		<td>Limitations</td>
	</tr>
	<tr>
		<td>Stage 5:</td> 
		<td>Raise awareness within development teams about all SAST tools and provide training for effective use of security tools from the very beginning of development.</br>Evaluation of well-defined Security Exception procedure and document </td></td>
		<td>Permissions</td>
		<td>Preparing development teams use SAST tools in pre-commit check.</br></br>
Implement continuous monitoring to track the effectiveness of SAST and other security practices.</br>
Establish feedback loops where security findings are continuously fed back into development.</br>
Regularly review and refine SAST processes and rules based on feedback and emerging threats.</br>
Promote a culture where security is everyone’s responsibility and integrated into daily activities.</br></td>
		<td>Limitations</td>
	</tr>
</table>
