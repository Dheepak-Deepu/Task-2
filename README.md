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
| **Sender Email** | support@secure-paypal.com (suspicious domain resembling PayPal)              |
| **Return Path**  | Did not match trusted sender domain (spoofed)                               |
| **SPF Check**    | Failed — domain not authorized to send emails                                |
| **Suspicious Link** | http://paypal.verify-secureaccount.com — does not belong to PayPal         |
| **Urgent Language** | “Your account will be suspended unless you act immediately.”               |
| **Grammar Issues** | Minor errors and lack of personalization (e.g., “Dear user”)                |



# Phishing Indicators Identified

- ✅ Spoofed sender domain
- ✅ Failed SPF authentication
- ✅ Suspicious URL disguised as a PayPal link
- ✅ Threatening tone to induce urgency
- ✅ Generic message with no personal identifiers



# Conclusion

The email is clearly a **phishing attempt** designed to trick users into revealing login credentials.  
By impersonating PayPal and using fake urgency, it attempts to bypass user suspicion.



# 📁 Repository Contents

```
cyber-security-task-2/
├── README.md                                      # This report
├── Sample Email                                   # Original Email
├── Sample Email - Original Message.txt            # Raw sample email content
└── Report - MX Toolbox                            # MXToolbox output screenshot
```
