# Secure Design Principles Cheat Sheet

## Introduction

Security design principles and concepts serve as the foundation for engineering trustworthy secure systems, including their constituent subsystems and components. These principles and concepts represent research, development, and application experience starting with the early incorporation of security mechanisms for trusted operating systems, to today’s wide variety of fully networked, distributed, mobile, and virtual computing components, environments, and systems. The principles and concepts are intended to be universally applicable across this broad range of systems, as well as new systems as they emerge and mature. [NIST 800-160 Appendix F]

## Main Sections

### Least-Privilege

The principle of least privilege states that each component should be allocated sufficient privileges to accomplish its specified functions, but no more. This limits the scope of the component’s actions, which has two desirable effects: the security impact of a failure, corruption, or misuse of the component will have a minimized security impact; and the security analysis of the component will be simplified. [NIST]

(More detail)

### Defense-in-Depth

The principle of defense in depth suggests that where one control would be reasonable, more controls that approach risks in different fashions are better. Controls, when used in depth, can make severe vulnerabilities extraordinarily difficult to exploit and thus unlikely to occur. [OWASP]

(More detail)

### Least Common Mechanism

The principle of least common mechanism states that the amount of mechanism common to more than one user and depended on by all users should be minimized [Popek74]. This implies that different components of a system should refrain from using the same mechanism to access a system resource. [NIST]

(More detail)

### Acceptable Security

The principle of acceptable security requires that the level of privacy and performance the system provides should be consistent with the users’ expectations. The perception of personal privacy may affect user behavior, morale, and effectiveness. Based on the organizational privacy policy and the system design, users should be able to restrict their actions to protect their privacy. [NIST]

(More detail)

### Minimize Attack Surface

Every feature that is added to an application adds a certain amount of risk to the overall application. The aim for secure development is to reduce the overall risk by reducing the attack surface area. [OWASP]

(More detail)

### Separation of Duties

A key fraud control is separation of duties. For example, someone who requests a computer cannot also sign for it, nor should they directly receive the computer. This prevents the user from requesting many computers, and claiming they never arrived. Certain roles have different levels of trust than normal users. In particular, administrators are different from normal users. In general, administrators should not be users of the application. [OWASP]

(More detail)

### Reduced Complexity

The principle of reduced complexity states that the system design should be as simple and small as possible. A small and simple design will be more understandable, more analyzable, and less prone to error. This principle applies to any aspect of a system, but it has particular importance for security due to the various analyses performed to obtain evidence about the emergent security property of the system. [NIST]

(More detail)

### Secure Failure and Recovery

The principle of secure failure and recovery states that neither a failure in a system function or mechanism nor any recovery action in response to failure should lead to a violation of security policy. This principle parallels the principle of continuous protection to ensure that a system is capable of detecting (within limits) actual and impending failure at any stage of its operation and to take appropriate steps to ensure that security policies are not violated. [NIST]

(More detail)

### Secure Defaults

The principle of secure defaults states that the default configuration of a system (to include its constituent subsystems, components, and mechanisms) reflects a restrictive and conservative enforcement of security policy. The principle of secure defaults applies to the initial configuration of a system as well as to the security engineering and design of access control and other security functions that should follow a “deny unless explicitly authorized” strategy. [NIST]

(More detail)

### Accountability and Traceability

The principle of accountability and traceability states that it must be possible to trace security relevant actions (i.e., subject-object interactions) to the entity on whose behalf the action is being taken. This principle requires a trustworthy infrastructure that can record details about actions that affect system security (e.g., an audit subsystem). To do this, the system must not only be able to uniquely identify the entity on whose behalf the action is being carried out, but also record the relevant sequence of actions that are carried out. [NIST]

(More detail)

## References

NIST SP 800-160v1: Appendix F
[https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-160v1.pdf](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-160v1.pdf)

There used to be a section from the old dev guide.
[https://github.com/OWASP/DevGuide/blob/master/02-Design/01-Principles%20of%20Security%20Engineering.md](https://github.com/OWASP/DevGuide/blob/master/02-Design/01-Principles%20of%20Security%20Engineering.md)

A variant of guidance from the UK
[https://www.ncsc.gov.uk/collection/cyber-security-design-principles/cyber-security-design-principles](https://www.ncsc.gov.uk/collection/cyber-security-design-principles/cyber-security-design-principles)

CISA Archive
[https://us-cert.cisa.gov/bsi/articles/knowledge/principles/design-principles](https://us-cert.cisa.gov/bsi/articles/knowledge/principles/design-principles)

Older OWASP References
[https://wiki.owasp.org/index.php/Security_by_Design_Principles](https://wiki.owasp.org/index.php/Security_by_Design_Principles)