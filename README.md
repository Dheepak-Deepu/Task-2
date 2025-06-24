# Task 2: Phishing Email Analysis Report

##  Tools Used

- **Email Client**: Gmail  
- **Header Analyzer**: [MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)


# Step-by-Step Procedure

1. *Opened Sample Email*  
   Accessed a suspicious email in my Gmail inbox that appeared to be a phishing attempt.

2. *Downloaded Original Email Header* 
   Used Gmail’s “Show Original” option to view the raw email headers and copied the entire content.

3. *Analyzed Header on MXToolbox* 
   - Pasted the copied header into MXToolbox's header analyzer.
   - Reviewed results related to SPF, DKIM, IP, and server paths.


# Key Observations

| Attribute         | Observation                                                                 |
|------------------|------------------------------------------------------------------------------|
| **Sender Email** | marketing@smt.plusoasis.com (suspicious and non-official)                   |
| **Return Path**  | Different from domain in "From" address                                      |
| **SPF Check**    | Failed / Misaligned (issues found in SPF alignment)                         |
| **Suspicious Link** | Not directly mentioned but inferred from phishing context                   |
| **Urgent Language** | “Your card is waiting. Complete your application now.”                     |
| **Grammar Issues** | Use of generic language like "Dear Sir/Mam", lacks personalization          |

# Phishing Indicators Identified

- ✅ Spoofed or untrusted sender domain  
- ✅ SPF misalignment and issues in email authentication  
- ✅ Misleading or urgency-based subject line  
- ✅ Absence of personalization  
- ✅ Suspicious overall context and generic greeting

# Conclusion

The email is a **phishing attempt** trying to mislead users into clicking potentially harmful links or entering personal information.


# Repository Contents

```
cyber-security-task-2/
├── README.md                                      # This report
├── Sample Email                                   # Original Email
├── Sample Email - Original Message.txt            # Raw sample email content
└── Report - MX Toolbox                            # MXToolbox output screenshot
└── DKIM Test Report                               # Record which stores the sender's public key
```
