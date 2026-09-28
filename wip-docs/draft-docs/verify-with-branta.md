---
hidden: true
---

# Verify with Branta







***



## Verify with Branta <a href="#verify-with-branta" id="verify-with-branta"></a>

_Authoritative address verification for every Lightning payment on Lightning Bounties._

### Overview <a href="#overview" id="overview"></a>

`Verify with Branta` is an **optional yet highly-recommended safety check** that lets you confirm a BOLT-11 invoice before you pay it on Lightning Bounties. Powered by Branta’s **Guardrail** service, the link under each deposit form opens a separate, read-only page that validates the invoice hash and destination against Branta’s independent database.

\
If the data match, the page displays a green “Verified” banner; if anything is off, you will see a red warning so you can abort the payment.

> **Why it matters**: Lightning payments are final. Clipboard-swapping malware, malicious browser extensions or compromised Wi-Fi can silently replace an invoice. `Verify with Branta` gives you a second source of truth so you can transact with confidence.

### Key Benefits <a href="#key-benefits" id="key-benefits"></a>

| Benefit                                          | What it means for you                                                                                      |
| ------------------------------------------------ | ---------------------------------------------------------------------------------------------------------- |
| **Protection against man-in-the-middle attacks** | Detect invoice tampering before funds leave your wallet.                                                   |
| **Multi-device cross-check**                     | Open the Branta link on a second phone or computer for added assurance—your main browser cannot interfere. |
| **Zero-friction UX**                             | One click; no account, no extra data entry, no delay.                                                      |
| **Independent verification**                     | Branta runs on infrastructure outside Lightning Bounties, eliminating single-point-of-failure risks.       |
| **Privacy-first design**                         | Branta never sees your IP-linked wallet data; it only checks the invoice string you already have.          |

### How to Use Verify with Branta <a href="#how-to-use-verify-with-branta" id="how-to-use-verify-with-branta"></a>

1. Generate or locate the BOLT-11 invoice in Lightning Bounties’ **Add Reward** modal.
2. **Click “Verify Invoice - Branta”** below the QR code. A new tab opens.
3. Confirm you see a **green “Verified” status** and that the amount and memo match what Lightning Bounties shows.
4. Pay the invoice from your Lightning wallet.

> **Placeholder for Screenshot 1**\
> &#xNAN;_&#x44;escription_: Deposit modal displaying QR code, invoice string and the _Verify Invoice - Branta_ link.\
> &#xNAN;_&#x43;aption_: “Lightning Bounties deposit form with Branta verification option.”

> **Placeholder for Screenshot 2**\
> &#xNAN;_&#x44;escription_: Branta Guardrail page showing a green banner and “Lightning Bounties verified since block XXXX.”\
> &#xNAN;_&#x43;aption_: “Successful verification of a Lightning Bounties invoice on Branta.”

### Best-Practice Scenarios <a href="#best-practice-scenarios" id="best-practice-scenarios"></a>

| Scenario                              | Recommended Action                                                   |
| ------------------------------------- | -------------------------------------------------------------------- |
| High-value reward deposits            | Always run Branta verification before paying.                        |
| Using public or shared Wi-Fi          | Verify on a second device (phone or offline laptop).                 |
| First-time user of Lightning Bounties | Click the link to experience the safety flow.                        |
| Suspicious browser behaviour          | Pause, copy the invoice, open Branta in a different browser profile. |

### Security Model at a Glance <a href="#security-model-at-a-glance" id="security-model-at-a-glance"></a>

| Without Guardrail [1](https://www.branta.pro/guardrail) | With Guardrail [1](https://www.branta.pro/guardrail) |
| ------------------------------------------------------- | ---------------------------------------------------- |
| Users cannot confirm the true recipient.                | Users get a cryptographic match on destination.      |
| Single point of failure (website).                      | Independent verification host.                       |
| Fake invoices may go unnoticed.                         | Mismatched invoices trigger a red alert.             |

### Tutorial: Adding Rewards Without Logging In (Anonymous Deposits) <a href="#tutorial-adding-rewards-without-logging-in-anonymo" id="tutorial-adding-rewards-without-logging-in-anonymo"></a>

Lightning Bounties lets anyone top-up an existing bounty—even without a platform account. Here’s how to combine that flow with Branta verification for maximum safety.

1. **Navigate to the bounty page** on `app.lightningbounties.com`.
2. Click **“Add Reward”**.
3. **Enter amount** in sats and adjust _Advanced Settings_ if needed (e.g., lock time).
4. When the deposit modal appears, **copy or scan the invoice**.
5. **Click “Verify Invoice - Branta.”**
6. After you see a green verification, **pay the invoice** from any Lightning wallet.
7. Refresh the bounty page to confirm your reward was added.

For a full walkthrough of anonymous rewards, see Lightning Bounties Docs → _Adding Anonymous Rewards to a Bounty_.

> **Placeholder for Screenshot 3**\
> &#xNAN;_&#x44;escription_: Anonymous Add-Reward flow highlighting the amount picker and Branta link.\
> &#xNAN;_&#x43;aption_: “Anonymous contributor adding sats with Branta verification.”

### Frequently Asked Questions <a href="#frequently-asked-questions" id="frequently-asked-questions"></a>

**Is Branta mandatory?**\
No. Payments succeed even if you skip verification, but you lose the extra security layer.

**Does Branta ever see my private keys or wallet data?**\
Never. Branta checks only the public invoice string you already hold 2.

**What happens if Branta shows a red warning?**\
Do **not** pay. Generate a new invoice on Lightning Bounties or contact support.

**Can I verify on mobile?**\
Yes. Copy the invoice URL or scan the QR on a separate phone and open the link in any browser.

### Summary <a href="#summary" id="summary"></a>

`Verify with Branta` brings Guardrail’s industry-leading address verification directly into every Lightning Bounties payment flow. One click turns irreversible Bitcoin transfers from stressful to secure—no logins, no extra cost, just peace of mind [1](https://www.branta.pro/guardrail)2.

References\
[1](https://www.branta.pro/guardrail) branta.pro/guardrail\
2 brantaops.substack.com/p/lightning-bounties-secures-bolt-11

1. [https://www.branta.pro/guardrail](https://www.branta.pro/guardrail)
2. [https://www.youtube.com/watch?v=zEALcfaL\_VI](https://www.youtube.com/watch?v=zEALcfaL_VI)
3. [https://pplx-res.cloudinary.com/image/private/user\_uploads/34400399/8620b721-7cb8-4024-9ab8-c02441e2576d/verifyWithBrantaScreenShot.jpg](https://pplx-res.cloudinary.com/image/private/user_uploads/34400399/8620b721-7cb8-4024-9ab8-c02441e2576d/verifyWithBrantaScreenShot.jpg)
4. [https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/34400399/9ac01c75-24bf-49c0-b3a9-67633313975e/Verify\_With\_Branta.mp4](https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/attachments/34400399/9ac01c75-24bf-49c0-b3a9-67633313975e/Verify_With_Branta.mp4)
5. [https://blog.lightningbounties.com](https://blog.lightningbounties.com/)
6. [https://www.custompitch.com/projects/branta](https://www.custompitch.com/projects/branta)
7. [https://www.branta.pro/network](https://www.branta.pro/network)
8. [https://www.youtube.com/watch?v=yA4SUImqJBs](https://www.youtube.com/watch?v=yA4SUImqJBs)
9. [https://www.branta.pro/guardrail+](https://www.branta.pro/guardrail+)
10. [http://jimmccormac.blogspot.com](http://jimmccormac.blogspot.com/)
11. [https://twitter.com/BrantaOps/status/1838954044368232645](https://twitter.com/BrantaOps/status/1838954044368232645)
12. [https://www.financial-news.co.uk/branta-and-amboss-partner-for-safer-bitcoin-transactions/](https://www.financial-news.co.uk/branta-and-amboss-partner-for-safer-bitcoin-transactions/)
13. [https://blog.lightningbounties.com/top-builder-2025/top-builder-x-lightning-bounties/top-builder-teams/branta-guardrails-for-bitcoin-and-lightning](https://blog.lightningbounties.com/top-builder-2025/top-builder-x-lightning-bounties/top-builder-teams/branta-guardrails-for-bitcoin-and-lightning)
14. [https://brantaops.substack.com/p/lightning-bounties-secures-bolt-11](https://brantaops.substack.com/p/lightning-bounties-secures-bolt-11)
15. [https://docs.lightningbounties.com/docs/getting-started/managing-your-bounty/add-reward-to-an-existing-bounty](https://docs.lightningbounties.com/docs/getting-started/managing-your-bounty/add-reward-to-an-existing-bounty)





***



## Verify with Branta <a href="#verify-with-branta" id="verify-with-branta"></a>

### Overview <a href="#overview" id="overview"></a>

**Verify with Branta** is an **optional yet highly-recommended safety check** that lets you confirm a BOLT-11 invoice before you pay it on Lightning Bounties. Powered by Branta's **Guardrail** service, this verification link appears under each payment form and opens a separate, read-only page that validates the invoice hash and destination against Branta's independent database.

{Screenshot showing Lightning Bounties deposit modal displaying QR code, invoice string and the Verify Invoice - Branta link}

### Why Invoice Verification Matters <a href="#why-invoice-verification-matters" id="why-invoice-verification-matters"></a>

**Lightning payments are final**. Once you send Bitcoin through the Lightning Network, there's no way to reverse the transaction. This permanence makes verification crucial because various attack vectors can compromise your payment:

* **Clipboard-swapping malware** can silently replace invoices with attacker addresses120
* **Malicious browser extensions** may intercept and modify payment data
* **Compromised Wi-Fi networks** could perform man-in-the-middle attacks120
* **Phishing websites** might display fraudulent payment requests

**Verify with Branta gives you a second source of truth** so you can transact with confidence12022.

{Image showing various attack vectors that Branta verification protects against, including malware, browser extensions, and network attacks}

### Key Benefits of Branta Verification <a href="#key-benefits-of-branta-verification" id="key-benefits-of-branta-verification"></a>

| Benefit                                          | What it means for you                                                                                        |
| ------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| **Protection against man-in-the-middle attacks** | Detect invoice tampering before funds leave your wallet120                                                   |
| **Multi-device cross-check**                     | Open the Branta link on a second phone or computer for added assurance—your main browser cannot interfere120 |
| **Zero-friction UX**                             | One click; no account, no extra data entry, no delay120                                                      |
| **Independent verification**                     | Branta runs on infrastructure outside Lightning Bounties, eliminating single-point-of-failure risks120       |
| **Privacy-first design**                         | Branta never sees your IP-linked wallet data; it only checks the invoice string you already have120          |

### How Branta Guardrail Works <a href="#how-branta-guardrail-works" id="how-branta-guardrail-works"></a>

Branta's **Guardrail service** provides2027:

### One-Click Verification

* **Verify invoices, checkouts and deposits** before paying in Bitcoin or Lightning
* **Cross-device verification** in less than 2 seconds
* **No required apps or logins** - maintains zero learning curve
* **Privacy preservation** throughout the verification process

### Security Model Comparison

| Without Guardrail                       | With Guardrail                                 |
| --------------------------------------- | ---------------------------------------------- |
| Users cannot confirm the true recipient | Users get a cryptographic match on destination |
| Single point of failure (website)       | Independent verification host                  |
| Fake invoices may go unnoticed          | Mismatched invoices trigger a red alert        |

{Diagram showing the security architecture difference between standard payments and Branta-protected payments}



### <mark style="background-color:red;">Step 1: Generate Your Lightning Invoice</mark>

{% stepper %}
{% step %}
#### **Navigate to the Lightning Bounties payment form** (deposit, add reward, etc.)


{% endstep %}

{% step %}
#### **Enter your contribution amount** and configure any advanced settings


{% endstep %}

{% step %}
#### **Click "Generate Invoice"** to create the BOLT-11 payment request


{% endstep %}

{% step %}
#### **Locate the QR code and invoice string** in the payment modal


{% endstep %}
{% endstepper %}

### <mark style="background-color:red;">Step 1: Generate Your Lightning Invoice</mark>

1. **Navigate to the Lightning Bounties payment form** (deposit, add reward, etc.)
2. **Enter your contribution amount** and configure any advanced settings
3. **Click "Generate Invoice"** to create the BOLT-11 payment request
4. **Locate the QR code and invoice string** in the payment modal

### Step 2: Access Branta Verification

1. **Click "Verify Invoice - Branta"** below the QR code
2. **A new browser tab opens** automatically to Branta's verification service
3. **Wait for verification process** to complete (usually 1-2 seconds)
4. **Review the verification results** on the Branta page

### Step 3: Confirm Verification Status

**Look for the green verification banner**:

* **Green "Verified" status** indicates the invoice is legitimate
* **Amount and memo match** what Lightning Bounties displays
* **Destination confirmed** as authentic Lightning Bounties address
* **Block height reference** shows when verification was recorded

{Screenshot showing Branta Guardrail page with green banner displaying "Lightning Bounties verified since block XXXX"}

### Step 4: Complete Your Payment

1. **Return to Lightning Bounties** payment page
2. **Open your Lightning wallet** with confidence
3. **Scan the QR code or paste the invoice**
4. **Send the payment** knowing it's verified and secure

### Lightning Bounties Integration <a href="#lightning-bounties-integration" id="lightning-bounties-integration"></a>

Lightning Bounties has **integrated Branta directly into their application** to provide **an unparalleled level of security** for users22. This partnership ensures that:

* **Every transaction** on Lightning Bounties can be verified
* **Client-side tampering** is easily detected (previously not possible)22
* **Non-matching BOLT-11 deposits** are flagged as suspect22
* **Any internet-connected device** can verify payments22

The integration appears in multiple contexts:

* **Deposit forms** when funding your account
* **Add reward modals** for contributing to bounties
* **Anonymous contribution flows** for users without accounts

{Screenshot showing the complete Lightning Bounties payment flow with integrated Branta verification option}

### Best-Practice Scenarios <a href="#best-practice-scenarios" id="best-practice-scenarios"></a>

| Scenario                                  | Recommended Action                                                   |
| ----------------------------------------- | -------------------------------------------------------------------- |
| **High-value reward deposits**            | Always run Branta verification before paying1                        |
| **Using public or shared Wi-Fi**          | Verify on a second device (phone or offline laptop)1                 |
| **First-time user of Lightning Bounties** | Click the link to experience the safety flow1                        |
| **Suspicious browser behaviour**          | Pause, copy the invoice, open Branta in a different browser profile1 |
| **Anonymous contributions**               | Especially important due to lack of account recovery options         |
| **Corporate contributions**               | Verify large amounts to protect company funds                        |

### Advanced Multi-Device Verification <a href="#advanced-multi-device-verification" id="advanced-multi-device-verification"></a>

For **maximum security on high-value contributions**:

### Two-Device Setup

1. **Generate invoice** on your primary device (computer/phone)
2. **Copy the BOLT-11 invoice string** to clipboard
3. **Open Branta verification** on a second device
4. **Paste and verify** the invoice independently
5. **Cross-check results** between both devices

### Offline Verification

1. **Copy invoice** on connected device
2. **Transfer to offline/airplane mode device** via QR code or manual typing
3. **Use offline device** to access Branta verification
4. **Compare results** before making payment online

This approach **bypasses malware and network level attacks** by using independent infrastructure2027.

{Image showing multi-device verification setup with phone and computer displaying matching verification results}

### Understanding Verification Results <a href="#understanding-verification-results" id="understanding-verification-results"></a>

### Green Verification Status

**Positive verification means**120:

* **Invoice destination confirmed** as legitimate Lightning Bounties address
* **Amount and memo validated** against Branta's database
* **No tampering detected** in the payment request
* **Safe to proceed** with payment

### Red Warning Status

**If Branta shows a red warning**1:

* **Do NOT pay the invoice** under any circumstances
* **Generate a new invoice** on Lightning Bounties
* **Contact Lightning Bounties support** if problems persist
* **Report suspicious activity** to help protect other users

### Verification Process Details

**Branta Guardrail checks**2027:

* **Invoice hash validation** against known legitimate addresses
* **Destination address verification** through cryptographic matching
* **Amount and memo validation** for consistency
* **Timestamp verification** to prevent replay attacks

### Technical Architecture <a href="#technical-architecture" id="technical-architecture"></a>

### Independent Infrastructure

**Branta operates separately** from Lightning Bounties120:

* **Different servers** and network infrastructure
* **Independent database** of verified addresses
* **Separate security protocols** and monitoring
* **Redundant verification** pathways

### Cryptographic Validation

**Guardrail service provides**20:

* **Hash-based verification** of invoice authenticity
* **Cryptographic matching** against known good addresses
* **Tamper detection** through digital signature validation
* **Real-time verification** with minimal latency

### Integration with Anonymous Contributions <a href="#integration-with-anonymous-contributions" id="integration-with-anonymous-contributions"></a>

**Branta verification is especially critical** for anonymous contributions because:

* **No account recovery options** if payments go to wrong addresses
* **Limited dispute resolution** without platform account
* **Higher risk exposure** due to lack of contribution tracking
* **No direct support channel** for payment issues

The **combination of anonymous access and Branta verification** provides the perfect balance of privacy and security22.

### Business Benefits for Lightning Bounties <a href="#business-benefits-for-lightning-bounties" id="business-benefits-for-lightning-bounties"></a>

By integrating Branta, Lightning Bounties is positioned to2027:

* **Increase brand trust & loyalty** through enhanced security
* **Unlock new lanes of commerce/transactions** by reducing payment anxiety
* **Gracefully withstand cyber exploits** directed at their platform
* **Gracefully withstand cyber exploits** directed at their customers

This creates a **win-win-win scenario**: the platform wins, end users win, and Bitcoin wins20.

### Privacy and Data Protection <a href="#privacy-and-data-protection" id="privacy-and-data-protection"></a>

### Privacy-First Design

**Branta's privacy approach**120:

* **No IP tracking** or user identification
* **No wallet data collection** or storage
* **Invoice-only verification** without personal information
* **Minimal data retention** policies

### Data Security

**Protection measures include**:

* **Encrypted communication** for all verification requests
* **No persistent storage** of verification data
* **Anonymized processing** of invoice verification
* **Regular security audits** and updates

### Frequently Asked Questions <a href="#frequently-asked-questions" id="frequently-asked-questions"></a>

**Is Branta mandatory?**\
No. Payments succeed even if you skip verification, but you lose the extra security layer that protects against fraud and technical attacks.

**Does Branta ever see my private keys or wallet data?**\
Never. Branta checks only the public invoice string you already hold. Your wallet private keys, transaction history, and personal data remain completely private.

**What happens if Branta shows a red warning?**\
**Stop immediately**. Do **not** pay any invoice that fails Branta verification. Generate a new invoice on Lightning Bounties or contact support for assistance.

**Can I verify on mobile devices?**\
**Yes**. Copy the invoice URL or scan the QR on a separate phone and open the Branta verification link in any mobile browser.

**How does Branta protect against sophisticated attacks?**\
Branta provides **independent verification infrastructure** separate from Lightning Bounties, making it impossible for attackers to compromise both systems simultaneously. This creates a robust defense against even advanced attack scenarios.

### Tutorial: Safe Anonymous Contributions <a href="#tutorial-safe-anonymous-contributions" id="tutorial-safe-anonymous-contributions"></a>

### Complete Anonymous Safety Flow

1. **Navigate to bounty page** on `app.lightningbounties.com`
2. **Click "Add Reward"** without logging in
3. **Enter amount** and configure settings
4. **Generate Lightning invoice**
5. **Click "Verify Invoice - Branta"**&#x31;
6. **Confirm green verification** status20
7. **Cross-check amount and memo** details
8. **Pay invoice** from Lightning wallet
9. **Refresh bounty page** to confirm contribution

{Screenshot showing anonymous Add-Reward flow highlighting the amount picker and Branta verification link}

### Summary <a href="#summary" id="summary"></a>

**Verify with Branta** brings **Guardrail's industry-leading address verification** directly into every Lightning Bounties payment flow12022. One click turns irreversible Bitcoin transfers from stressful to secure—no logins, no extra cost, just peace of mind when contributing to open-source development.

The service protects against the most common attack vectors in Bitcoin payments while maintaining Lightning Bounties' core principle of **minimal friction and maximum accessibility**420. Whether you're making anonymous contributions or funding large bounties, Branta verification ensures your Bitcoin goes exactly where you intend it to go.

**Key takeaways**:

* **Lightning payments are final** - verification prevents costly mistakes120
* **Independent infrastructure** eliminates single points of failure20
* **Zero friction integration** maintains Lightning Bounties' user experience20
* **Privacy preservation** throughout the verification process120
* **Multi-device verification** provides maximum security for high-value transactions1

{Image showing the complete secure payment flow from invoice generation through Branta verification to successful contribution}

By integrating independent verification into the contribution process, Lightning Bounties demonstrates its commitment to user security while maintaining the frictionless experience that makes **Bitcoin-powered open-source funding accessible to everyone**



### Step 3: Configure Your Anonymous Reward

1. **Enter the amount** in sats you want to contribute8
2. **Adjust Advanced Settings** if needed:
   * **Set lock time** for your contribution (optional)8
   * **Review payment terms** and conditions
3. **Confirm your contribution details** before proceeding



1. **Click "Add Reward"** on the bounty detail page
2. **No login required** - the anonymous funding modal will appear
3. **Review the issue details** to confirm this is the bounty you want to support



####

### Implement [Branta Security Verification](https://brantaops.substack.com/p/lightning-bounties-secures-bolt-11)

**Essential security step**

1. **Click "Verify Invoice - Branta"** link below QR code
2. **New browser tab opens** to Branta's independent verification service
3. **Confirm green "Verified" status** appears
4. **Cross-check payment details**:
   * Amount matches your intended contribution
   * Recipient is Lightning Bounties
   * Memo corresponds to correct bounty

<figure><img src="../../.gitbook/assets/verifyWithBrantaScreenShot.JPG" alt="Screenshot showing generated Lightning invoice with QR code, BOLT-11 string, and payment details"><figcaption><p>Screenshot showing generated Lightning invoice with QR code, BOLT-11 string, and payment details</p></figcaption></figure>

{% hint style="info" %}
**Why Branta verification matters**:

* **Prevents man-in-the-middle attacks** that could redirect payments
* **Provides independent confirmation** outside Lightning Bounties infrastructure
* **Protects against clipboard malware** and browser extension interference
* **Offers multi-device verification** capability for high-value contributions
{% endhint %}

<div><figure><img src="../../.gitbook/assets/addressVerified.jfif" alt=""><figcaption><p><span data-gb-custom-inline data-tag="emoji" data-code="2705">✅</span> <strong>Address Verified</strong> <span data-gb-custom-inline data-tag="emoji" data-code="2705">✅</span><strong>OK TO SEND FUNDS</strong> <span data-gb-custom-inline data-tag="emoji" data-code="2705">✅</span></p></figcaption></figure> <figure><img src="../../.gitbook/assets/addressNotVerified.jfif" alt=""><figcaption><p>⛔ <strong>Address Not Verified</strong> ⛔ <strong>DO NOT SEND FUNDS</strong> ⛔</p></figcaption></figure></div>

<sub>_This_</sub><sub>_&#x20;_</sub><sub>_**optional yet highly-recommended safety check**_</sub><sub>_&#x20;_</sub><sub>_is especially critical for no-login users who lack account-based recovery options_</sub>

### Pay the Invoice with your Lightning Wallet&#x20;

A [BOLT 11 Lightning invoice ](https://www.whatisbitcoin.com/lightning-network/bolt-11-vs-bolt-12)and QR code will appear.

* Open your preferred [Lightning wallet](https://docs.lightningbounties.com/docs/resources/frequently-asked-questions/lightning-bounties-faqs#what-lightning-wallets-can-i-use) (Phoenix, Muun, Breez, Wallet of Satoshi, etc.).
* Scan the QR code or paste the invoice string.
* **Verify payment details** in your wallet interface
* **Confirm the payment**
* **Receive payment confirmation** in your wallet

<figure><img src="../../.gitbook/assets/verifyWithBrantaScreenShot.JPG" alt="Screenshot showing generated Lightning invoice with QR code, BOLT-11 string, and payment details"><figcaption><p>Screenshot showing generated Lightning invoice with QR code, BOLT-11 string, and payment details</p></figcaption></figure>

### Verify Contribution Success

1. **Return to bounty page** and refresh
2. **Confirm increased total reward** amount
3. **Verify contribution was processed** successfully
4. **Note updated bounty funding** for community awareness

The platform provides **real-time payment tracking** and **transparent reward systems**

<figure><img src="../../.gitbook/assets/image (69).png" alt="Screenshot of a Pop-up reading &#x22;Payment received; reward added! Refreshing in 5 secs...&#x22;"><figcaption><p>Should See This pop-up</p></figcaption></figure>

**See who contributed at the bottom**

<div data-full-width="true"><figure><img src="../../.gitbook/assets/image (67).png" alt=""><figcaption><p>Scroll to the Bottom of The Bounty</p></figcaption></figure></div>

#### Your anonymous reward is now live!

<figure><img src="../../.gitbook/assets/image (66).png" alt=""><figcaption><p>Should See Image Above</p></figcaption></figure>

### Step-by-Step Anonymous Reward Process

### Step 1: Navigate to the Bounty

1. **Visit** `app.lightningbounties.com`
2. **Browse the bounty feed** to find the issue you want to support[5](https://docs.lightningbounties.com/docs/getting-started/solving-a-bounty/looking-for-a-project-to-get-rewarded)
3. **Click on the bounty card** to view full details
4. **Verify the bounty is still active** (no trophy icon indicates it's unsolved)[5](https://docs.lightningbounties.com/docs/getting-started/solving-a-bounty/looking-for-a-project-to-get-rewarded)

{Screenshot showing the bounty feed with various active bounties highlighted}

### Step 2: Access the Add Reward Feature

1. **Click "Add Reward"** on the bounty detail page
2. **No login required** - the anonymous funding modal will appear
3. **Review the issue details** to confirm this is the bounty you want to support

### Step 3: Configure Your Anonymous Reward

1. **Enter the amount** in sats you want to contribute8
2. **Adjust Advanced Settings** if needed:
   * **Set lock time** for your contribution (optional)8
   * **Review payment terms** and conditions
3. **Confirm your contribution details** before proceeding

{Screenshot showing the anonymous reward configuration modal with amount input and advanced settings}

### Step 4: Generate Payment Invoice

1. **Click to generate the Lightning invoice**
2. **Copy or scan the BOLT-11 invoice** that appears
3. **Note the payment amount and memo** for verification

### Step 5: Verify with Branta (Highly Recommended)

Before making your payment, **use Branta verification for maximum security**8:

1. **Click "Verify Invoice - Branta"** below the QR code8
2. **A new tab opens** showing Branta's verification page8
3. **Confirm you see a green "Verified" status**8
4. **Verify the amount and memo match** what Lightning Bounties shows8

{Screenshot showing the Branta verification page with green verified status}

This verification step is **especially important for anonymous contributions** because you won't have an account to track payment disputes.

### Step 6: Complete the Payment

1. **Open your Lightning wallet** (any Lightning-compatible wallet works)
2. **Paste the invoice** or scan the QR code
3. **Confirm the payment details** match your intended contribution
4. **Send the payment** - it should process within seconds

### Step 7: Verify Contribution Success

1. **Refresh the bounty page** after payment
2. **Check that the total bounty amount** has increased by your contribution
3. **Look for confirmation** that your reward was added successfully

{Screenshot showing the bounty page with updated total amount after anonymous contribution}

### Security Best Practices for Anonymous Rewards

### Payment Verification

* **Always use Branta verification** for invoice validation
* **Double-check payment amounts** before sending
* **Verify recipient details** match Lightning Bounties

### Network Security

* **Use secure networks** when making payments
* **Consider using a VPN** for additional privacy
* **Avoid public Wi-Fi** for payment transactions

### Multi-Device Verification

For high-value anonymous contributions8:

* **Open Branta verification on a second device** (phone or offline laptop)
* **Cross-check invoice details** on multiple devices
* **Confirm payment details** before final submission

