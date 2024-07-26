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
		<td><h4>Stage 1:</h4></td>
		<td>Basic Security Training. Provide initial security awareness training to development and operations teams. Introduce fundamental security concepts and common vulnerabilities.</td>
		<td>Ad Hoc Approach: Threat modeling is performed sporadically, often only when specific issues arise. Secure-SDLC is not adopted No collabration between Security Architects (Product Security Officer) and Development team Architects, project managers, stakeholders at design phase. Security Architecture Reviews and Threat Modeling are missing. All required documents for Threat Modeling are not available in Design phase.</td>
		<td>As per tech stack, identify Basic SAST tools (Source code analysis tool, Open Source Software/code tool). Source code analysis tools: Fortify, Coverity, Checkmarx, Veracode, Bandit, Cppcheck. Open Source Software tools: BlackDuck, Snyk, WhiteSource, OWASP Dependency-Check, Retire.js, Clair. Introduce developers to SAST tools and their benefits. Provide basic training on how to use SAST tools effectively.</td>
		<td>EDUCATE: Introduce teams to DAST tools and their benefits. Provide basic training on how to configure and use DAST tools effectively.</td>
	</tr>
	<tr>
		<td><h4>Stage 2:</h4></td>
		<td>Establish security requirements and policies. Document these requirements and ensure they are accessible to all teams. **Guideline Documents:** Input Parameter Validation Guidelines, Security Coding Guidelines, Sensitive Data Discovery Guidance for Development Teams. API/Web/Mobile/Thick Client/Hardware Security and Privacy Guidelines</td>
		<td>Adoption of standard methodologies such as STRIDE or DREAD. Create the awareness, Trainings and benifits of Threat Model and Security Architecture Reviews at design phase. Provide requirement details (Architectural Design Diagram, LLDD, HLDD etc.) of Threat Model and Security Architecture Reviews. High-Level Design Document should contain security objectives (e.g., confidentiality, integrity, availability). Low-Level Design Document (LLDD) should contain Access controls, authentication, and authorization mechanisms, Encryption and data protection requirements.</td>
		<td>Select and implement a SAST tool that fits the organization’s technology stack and needs. On top of basic SASt tools, identify Sensitive information disclosure tool, IaC tool and Malware scan tools. Sensitive information disclosure tools: GitLeaks, TruffleHog, git-secrets. IaC tools: Checkov, Aqua Security, kics (Keeping Infrastructure as Code Secure), Pulumi. Malware scan tools: Malwarebytes, Bitdefender, Norton, McAfee.</td>
		<td>IDENTIFY: Select and implement a DAST tool that fits the organization’s technology stack and needs. Integrate DAST into the testing environment to allow dynamic scans of running applications. This DAST will take care of common security exploits and provides results. DAST tools: OWASP ZAP proxy, Burpsuite pro, Burpsuite Enterprise.</td>
	</tr>
	<tr>
		<td><h4>Stage 3:</h4></td>
		<td>Provide ongoing security training to keep the teams updated on the latest threats and best practices. Encourage developers to take ownership of security by creating a security champions program. Introducing Tainings/Work Instructions. Security and Privacy Risk Management Procedure. Security and Privacy Risk Management SAST Work Instructions. Security and Privacy Risk Management DAST Work Instructions. Security and Privacy Test Cases Procedure. Cryptography and Key Management Standard</td>
		<td>Threat modeling is applied consistently across projects and systems. Collaboration between development, security, and operations teams. Regular reviews and updates of threat models based on new threats and changes.</td>
		<td>Integrate SAST tools into the CI/CD pipeline to ensure that security scans are performed automatically with every build. Set up automated notifications for vulnerabilities detected during SAST scans.</td>
		<td>INTEGRATE: Integrate DAST tools into the CI/CD pipeline to ensure that security scans are performed automatically with every build. Set up automated notifications for vulnerabilities detected during DAST scans.</td>
	</tr>
	<tr>
		<td><h4>Stage 4:</h4></td>
		<td>Security & Privacy touch point sessions. Involving in Release design and planning stage and overlook SAST status and CI-CD pipe lines. Insider Threat Mitigation Program Procedure. Open Source Software Vulnerability Management Procedure</td>
		<td>Use of advanced tools and techniques for threat modeling and risk assessment (Along with opensource Threat Model tools using professional Threat Model tools). Ongoing training and development for teams on advanced threat modeling techniques. Collect feedback from stakeholders and incorporate lessons learned into future threat modeling exercises.</td>
		<td>Ensure that all code, including third-party libraries and open-source components, is scanned by SAST tools. Regularly update SAST tools and their rule sets to cover the latest vulnerabilities. Develop necessary SAST gated builds. Promote the role of security champions within development teams who advocate for secure coding practices.</td>
		<td>ADD MORE: Ensure that all components of the application, including APIs and third-party integrations, are scanned by DAST tools. Regularly update DAST tools and their rule sets to cover the latest vulnerabilities. In addition to utilizing DAST tools, incorporate Interactive Application Security Testing (IAST) tools. IAST Tools: Develop Own Security automation framework, Synopsys Seeker, Acunetix At lease 20-30% of manual security efforts should be taken care by DAST/IAST tools.</td>
	</tr>
	<tr>
		<td><h4>Stage 5:</h4></td>
		<td>Raise awareness within development teams about all SAST tools and provide training for effective use of security tools from the very beginning of development. Evaluation of well-defined Security Exception procedure and document</td>
		<td>Security architecture reviews and Threat Model completion at Design level. If any gap is foung in Security Design, providing feedback (or Risk Track), conducting re-assesment on new disign. The output of Threat model will be discuss with Pentest Team (Scenarios which are testable at once feature/product is ready) and finalizing Security Test Stratergy document.</td>
		<td>Preparing development teams use SAST tools in pre-commit check. Implement continuous monitoring to track the effectiveness of SAST and other security practices. Establish feedback loops where security findings are continuously fed back into development. Regularly review and refine SAST processes and rules based on feedback and emerging threats. Promote a culture where security is everyone’s responsibility and integrated into daily activities.</td>
		<td>REDUCE MANUAL EFFORT: Implement continuous security monitoring to detect and respond to threats in real time. Establish feedback loops where security findings from DAST scans are continuously fed back into development. At lease 50% of manual security efforts should be taken care by DAST/IAST tools.</td>
	</tr>
</table>
































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
		<td>Ad Hoc Approach: Threat modeling is performed sporadically, often only when specific issues arise.
Secure-SDLC is not adopted 
No collabration between Security Architects (Product Security Officer) and Development team Architects, project managers, stakeholders at design phase.
Security Architecture Reviews and Threat Modeling are missing.
All required documents for Threat Modeling are not available in Design phase.</td>
		<td>As per tech stack, identify Basic SAST tools (Source code analysis tool, Open Source Software/code tool).</br>
Source code analysis tools: Fortify, Coverity, Checkmarx, Veracode, Bandit, Cppcheck.</br>
Open Source Software tools: BlackDuck, Snyk, WhiteSource, OWASP Dependency-Check, Retire.js, Clair.</br>
Introduce developers to SAST tools and their benefits.</br>
Provide basic training on how to use SAST tools effectively.</br></td>
		<td>EDUCATE:</br>
Introduce teams to DAST tools and their benefits.</br> 
Provide basic training on how to configure and use DAST tools effectively.</td>
	</tr>
	<tr>
		<td>Stage 2:</td> 
		<td>Establish security requirements and policies.</br>Document these requirements and ensure they are accessible to all teams.</br>**Guideline Documents:**</br>Input Parameter Validation Guidelines</br>Security Coding Guidelines</br>Sensitive Data Discovery Guidance for Development Teams</br>API/Web/Mobile/Thick Client/Hardware Security and Privacy Guidelines</td>
		<td>Adoption of standard methodologies such as STRIDE or DREAD.
Create the awareness, Trainings and benifits of Threat Model and Security Architecture Reviews at design phase.
Provide requirement details (Architectural Design Diagram, LLDD, HLDD etc.) of Threat Model and Security Architecture Reviews.
High-Level Design Document should contain security objectives (e.g., confidentiality, integrity, availability).
Low-Level Design Document (LLDD) should contain Access controls, authentication, and authorization mechanisms, Encryption and data protection requirements.</td>
		<td>Select and implement a SAST tool that fits the organization’s technology stack and needs.</br>
On top of basic SASt tools, identify Sensitive information disclosure tool, IaC tool and Malware scan tools.</br>
Sensitive information disclosure tools: GitLeaks, TruffleHog, git-secrets.</br>
IaC tools: Checkov, Aqua Security, kics (Keeping Infrastructure as Code Secure), Pulumi.</br>
Malware scan tools: Malwarebytes, Bitdefender, Norton, McAfee.</br></td>
		<td>IDENTIFY:</br>Select and implement a DAST tool that fits the organization’s technology stack and needs.</br>Integrate DAST into the testing environment to allow dynamic scans of running applications.</br>This DAST will take care of common security exploits and provides results.</br>DAST tools: OWASP ZAP proxy, Burpsuite pro, Burpsuite Enterprise.</td>
	</tr>
	<tr>
		<td>Stage 3:</td> 
		<td>Provide ongoing security training to keep the teams updated on the latest threats and best practices.</br>Encourage developers to take ownership of security by creating a security champions program.</br>Introducing Tainings/Work Instructions.</br>Security and Privacy Risk Management Procedure.</br>Security and Privacy Risk Management SAST Work Instructions.</br>Security and Privacy Risk Management DAST Work Instructions.</br>Security and Privacy Test Cases Procedure.</br>Cryptography and Key Management Standard</td>
		<td>Threat modeling is applied consistently across projects and systems.
Collaboration between development, security, and operations teams.
Regular reviews and updates of threat models based on new threats and changes.</td>
		<td>Integrate SAST tools into the CI/CD pipeline to ensure that security scans are performed automatically with every build.</br></br>
Set up automated notifications for vulnerabilities detected during SAST scans.</br></td>
		<td>INTEGRATE:</br> Integrate DAST tools into the CI/CD pipeline to ensure that security scans are performed automatically with every build.</br>Set up automated notifications for vulnerabilities detected during DAST scans.</br></td>
	</tr>
	<tr>
		<td>Stage 4:</td> 
		<td>Security & Privacy touch point sessions.</br>Involving in Release design and planning stage and overlook SAST status and CI-CD pipe lines</br>Insider Threat Mitigation Program Procedure</br>Open Source Software Vulnerability Management Procedure</td>
		<td>Use of advanced tools and techniques for threat modeling and risk assessment (Along with opensource Threat Model tools using professional Threat Model tools).
Ongoing training and development for teams on advanced threat modeling techniques.
Collect feedback from stakeholders and incorporate lessons learned into future threat modeling exercises.</td>
		<td>Ensure that all code, including third-party libraries and open-source components, is scanned by SAST tools.</br>
Regularly update SAST tools and their rule sets to cover the latest vulnerabilities.</br>
Develop necessary SAST gated builds.</br>
Promote the role of security champions within development teams who advocate for secure coding practices.</br></td>
		<td>ADD MORE:</br> Ensure that all components of the application, including APIs and third-party integrations, are scanned by DAST tools.</br>Regularly update DAST tools and their rule sets to cover the latest vulnerabilities.</br>In addition to utilizing DAST tools, incorporate Interactive Application Security Testing (IAST) tools.</br>IAST Tools: Develop Own Security automation framework, Synopsys Seeker, Acunetix</br>At lease 20-30% of manual security efforts should be taken care by DAST/IAST tools.</td>
	</tr>
	<tr>
		<td>Stage 5:</td> 
		<td>Raise awareness within development teams about all SAST tools and provide training for effective use of security tools from the very beginning of development.</br>Evaluation of well-defined Security Exception procedure and document </td></td>
		<td>Security architecture reviews and Threat Model completion at Design level.
If any gap is foung in Security Design, providing feedback (or Risk Track), conducting re-assesment on new disign.
The output of Threat model will be discuss with Pentest Team (Scenarios which are testable at once feature/product is ready) and finalizing Security Test Stratergy document.</td>
		<td>Preparing development teams use SAST tools in pre-commit check.</br></br>
Implement continuous monitoring to track the effectiveness of SAST and other security practices.</br>
Establish feedback loops where security findings are continuously fed back into development.</br>
Regularly review and refine SAST processes and rules based on feedback and emerging threats.</br>
Promote a culture where security is everyone’s responsibility and integrated into daily activities.</br></td>
		<td>REDUCE MANUAL EFFORT:</br>Implement continuous security monitoring to detect and respond to threats in real time.</br>Establish feedback loops where security findings from DAST scans are continuously fed back into development.</br>At lease 50% of manual security efforts should be taken care by DAST/IAST tools.</td>
	</tr>
</table>
