# Add Rewards to a Bounty without Login

Lightning Bounties' **no-login reward system** enables frictionless contributions to existing bounties, supporting the platform's goal of **minimal friction and maximum accessibility**. This feature allows anyone to instantly support open-source development without account creation barriers, embodying the principle that **it costs nothing to try**.

<figure><img src="../../../.gitbook/assets/image.png" alt="Lightning Bounties Product Emphasis"><figcaption><p>Lightning Bounties Product Emphasis</p></figcaption></figure>

### System Architecture Benefits <a href="#system-architecture-benefits" id="system-architecture-benefits"></a>

{% columns %}
{% column %}
<h3 align="center">Minimal Friction Design</h3>

**Effortless setup through:**

* **No installations required** - no plugins or software downloads
* **No account creation** - immediate access to funding features
* **Familiar GitHub integration** - leverages existing developer workflows


{% endcolumn %}

{% column %}
<h3 align="center">Global Accessibility Features</h3>

**The no-login system supports:**

* **No banking restrictions** - bypasses region-locked payment processors
* **Democratized funding** - anyone can contribute regardless of location
* **Censorship resistance** - peer-to-peer Bitcoin transactions
{% endcolumn %}
{% endcolumns %}

<div><figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Different Countries Contributing Without Barriers</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption><p>Bounty Flywheel</p></figcaption></figure></div>

### Understanding No-Login Contributions <a href="#understanding-no-login-contributions" id="understanding-no-login-contributions"></a>

The no-login system provides:

* **Instant access** to bounty funding without registration
* **Zero-friction contribution** process in under 30 seconds
* **Global accessibility** without banking restrictions
* **Privacy-first approach** for occasional contributors

This approach aligns with Lightning Bounties' core principle of **removing traditional barriers to open-source funding participation** while maintaining robust security

### Step-by-Step No-Login Process <a href="#step-by-step-no-login-process" id="step-by-step-no-login-process"></a>

{% hint style="info" %}
**No login required** - all bounties are visible to anonymous visitors
{% endhint %}

{% stepper %}
{% step %}
### **Visit** [**app.lightningbounties.com**](https://app.lightningbounties.com/) & <mark style="background-color:orange;">DO NOT Login With GitHub</mark>

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Non-logged-in state on Lightning Bounties Platform</p></figcaption></figure>
{% endstep %}

{% step %}
### **Browse the bounty feed** to find the issue you want to support

{% hint style="info" %}
**Verify the bounty is still active** (no trophy icon indicates it's unsolved)
{% endhint %}

<div data-full-width="true"><figure><img src="../../../.gitbook/assets/solvedCard.png" alt="No ⛔&#x22;Trophy&#x22; icon: Bounty is open for you to solve."><figcaption><p><strong>No</strong> ⛔<strong>"Trophy" icon:</strong> Bounty is open for you to solve.</p></figcaption></figure> <figure><img src="../../../.gitbook/assets/solvedCard (1).png" alt="&#x22;Trophy&#x22; 🏆 icon present: Bounty is solved &#x26; claimed."><figcaption><p><strong>"Trophy"</strong> 🏆 <strong>icon present: Bounty is solved &#x26; claimed.</strong></p></figcaption></figure></div>
{% endstep %}

{% step %}
### Click on the open bounty you want to support

<figure><img src="../../../.gitbook/assets/image (56).png" alt="No Trophy Means It&#x27;s Open to Add Rewards to"><figcaption><p>No Trophy Means It's Open to Add Rewards to</p></figcaption></figure>
{% endstep %}

{% step %}
### Create Anonymous Reward

**Enter the amount** in sats you want to contribute to the open bounty

<figure><img src="../../../.gitbook/assets/image (59).png" alt=""><figcaption><p>We'll use 5 sats for this demo but you'll likely commit more rewards</p></figcaption></figure>
{% endstep %}

{% step %}
### :warning: No Lock-Expiry on One-Time Rewards :warning:

When creating an anonymous one-time additional reward: you can't set a lock time.

Since you are not logged-in, this reward will not be tied to an account and you will not be able to be able to expire this award and recover the funds. **Thus there is no lock time available for this reward action.**

If you want to be able expire this award, you can log-in and post the reward as anonymous.

<figure><img src="../../../.gitbook/assets/image (68).png" alt=""><figcaption><p>Must log-In with GitHub to use the bounty lock time feature. </p></figcaption></figure>
{% endstep %}

{% step %}
### Click "Add Reward" - no authentication required

<figure><img src="../../../.gitbook/assets/image (63).png" alt="This button is available on every open bounty, whether you’re logged in or not!"><figcaption><p>This button is available on every open bounty, whether you’re logged in or not!</p></figcaption></figure>
{% endstep %}

{% step %}
### Implement [Branta Security Verification](https://brantaops.substack.com/p/lightning-bounties-secures-bolt-11)

**Essential security step**

1. **Click "Verify Invoice - Branta"** link below QR code
2. **New browser tab opens** to Branta's independent verification service
3. **Confirm green "Verified" status** appears
4. **Cross-check payment details**:
   * Amount matches your intended contribution
   * Recipient is Lightning Bounties
   * Memo corresponds to correct bounty

<figure><img src="../../../.gitbook/assets/verifyWithBrantaScreenShot.JPG" alt="Screenshot showing generated Lightning invoice with QR code, BOLT-11 string, and payment details"><figcaption><p>Screenshot showing generated Lightning invoice with QR code, BOLT-11 string, and payment details</p></figcaption></figure>

{% hint style="info" %}
**Why Branta verification matters**:

* **Prevents man-in-the-middle attacks** that could redirect payments
* **Provides independent confirmation** outside Lightning Bounties infrastructure
* **Protects against clipboard malware** and browser extension interference
* **Offers multi-device verification** capability for high-value contributions
{% endhint %}

<div><figure><img src="../../../.gitbook/assets/addressVerified.jfif" alt=""><figcaption><p><span data-gb-custom-inline data-tag="emoji" data-code="2705">✅</span> <strong>Address Verified</strong> <span data-gb-custom-inline data-tag="emoji" data-code="2705">✅</span><strong>OK TO SEND FUNDS</strong> <span data-gb-custom-inline data-tag="emoji" data-code="2705">✅</span></p></figcaption></figure> <figure><img src="../../../.gitbook/assets/addressNotVerified.jfif" alt=""><figcaption><p>⛔ <strong>Address Not Verified</strong> ⛔ <strong>DO NOT SEND FUNDS</strong> ⛔</p></figcaption></figure></div>

<sub>_This_</sub><sub>_&#x20;_</sub><sub>_**optional yet highly-recommended safety check**_</sub><sub>_&#x20;_</sub><sub>_is especially critical for no-login users who lack account-based recovery options_</sub>
{% endstep %}

{% step %}
### Pay the Invoice with your Lightning Wallet&#x20;

A [BOLT 11 Lightning invoice ](https://www.whatisbitcoin.com/lightning-network/bolt-11-vs-bolt-12)and QR code will appear.

* Open your preferred [Lightning wallet](https://docs.lightningbounties.com/docs/resources/frequently-asked-questions/lightning-bounties-faqs#what-lightning-wallets-can-i-use) (Phoenix, Muun, Breez, Wallet of Satoshi, etc.).
* Scan the QR code or paste the invoice string.
* **Verify payment details** in your wallet interface
* **Confirm the payment**
* **Receive payment confirmation** in your wallet

<figure><img src="../../../.gitbook/assets/verifyWithBrantaScreenShot.JPG" alt="Screenshot showing generated Lightning invoice with QR code, BOLT-11 string, and payment details"><figcaption><p>Screenshot showing generated Lightning invoice with QR code, BOLT-11 string, and payment details</p></figcaption></figure>
{% endstep %}

{% step %}
### Verify Contribution Success

1. **Return to bounty page** and refresh
2. **Confirm increased total reward** amount
3. **Verify contribution was processed** successfully
4. **Note updated bounty funding** for community awareness

The platform provides **real-time payment tracking** and **transparent reward systems**

<figure><img src="../../../.gitbook/assets/image (69).png" alt="Screenshot of a Pop-up reading &#x22;Payment received; reward added! Refreshing in 5 secs...&#x22;"><figcaption><p>Should See This pop-up</p></figcaption></figure>

**See who contributed at the bottom**

<div data-full-width="true"><figure><img src="../../../.gitbook/assets/image (67).png" alt=""><figcaption><p>Scroll to the Bottom of The Bounty</p></figcaption></figure></div>

#### Your anonymous reward is now live!
{% endstep %}

{% step %}
<figure><img src="../../../.gitbook/assets/image (66).png" alt=""><figcaption><p>Should See Image Above</p></figcaption></figure>
{% endstep %}
{% endstepper %}

***

### Summary <a href="#summary" id="summary"></a>

The no-login reward system exemplifies Lightning Bounties' commitment to **frictionless, accessible, and innovative** open-source funding. By removing traditional barriers while maintaining robust security through **Branta verification**, this feature enables anyone to instantly support the open-source development they care about.

This approach creates a **global bounty aggregator** that truly democratizes software development funding, making it possible for anyone, anywhere to contribute to the projects that matter most.
