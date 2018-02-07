---
id: Editing-Scope
title: Editing Scope
---
Your Scope is a collection of assets you want hackers to hack on.

To view and edit your existing scope: 
1. Go to the Scope section in your program's **Settings** > **Program** > **Policy & Scope**.

![Scope image 1](https://support.hackerone.com/hc/article_attachments/115009968543/Screen_Shot_2017-06-14_at_2.49.51_PM.png)

2. Click on **Add asset**. It will bring you to this page:
![Scope image 2](https://hackerone.zendesk.com/hc/article_attachments/115009968563/Screen_Shot_2017-06-14_at_2.51.46_PM.png)

3. Fill out the different fields. For each asset, you can fill out:

Option | Detail
----- | -----
Types | The asset type. <br>You an choose from these options: CIDR, Domain, iOS: App Store, iOS: Testflight, iOS: .ipa, Android: Play Store, Android: .apk, Windows: Microsoft Store, Source Code, Executable, Hardware/loT, Other.
Identifier | How hackers will know that they are at the correct asset that you specified. 
Eligibility for Submission | Whether you want hackers to submit to reports about this asset. If "no", hackers will see the asset on a report form with a red warning, and will not be able to submit reports marked for this asset.
Eligibility for Bounty | Whether you intend on providing bounties for this Asset or not. If you have a mixed Bug Bounty - Vulnerability Disclosure program, you will want to explicitly mark the Assets you will or will not pay for. This is also surfaced to hackers on both your team profile and the report submission form.
Environmental Score | Adjust the severity of each vulnerability submission based on the Environment by specifying the maximum impact to Confidentiality, Integrity, or Availability of that Asset's data. You can read more about our CVSS implementation here: How does HackerOne recommend determining Severity?
Instruction | If you have any detail descriptions or comments on the Asset, this field will surface that on both your program profile page and your report submission form.

## Best Practices for Setting up Your Scope
* **Provide granularity**
  * The more defined each asset is, the less room there is for misunderstanding. Avoid setting a wildcard to encapsulate different domains into one asset, e.g., keep your `blog.yourprogram.com` distinct from `secure.yourprogram.com`.
* **List Assets that are out of scope**.
  * It is perfectly fine, normal, and very encouraged, to have items that are out of scope. Do you have a completely isolated "affiliated site" maintained by a third party? List that as out of scope. No surprises for the hacker that spent hours hacking it, no surprises for you trying to explain "We do not own that property" after the fact.
  * If possible, explain why in the instructions field.
* **If you offer a bug bounty, make it clear which assets it is applicable to**. 
  * It is a common best practice to only offer bug bounties in specific assets, and to slowly expand that list over time. Set proper expectations with hackers by explicitly white-listing those assets that are eligible for bounties.
  * If possible, explain why in the instructions field. Over communication helps prevent future disagreements. 
* **Set the Environmental Score for the Asset**.
  * Confidentiality: Whether the data being obtained is actually confidential to their business, i.e, if there is a business risk when the data is leaked.
  * Integrity: What the business risk is if the data is modified
  * Availability: Business risk depending on if the component is on or offline
  * Not all of your Assets are created equal. You should take the time to assess potential business impact and configure these fields in order to:
    * Create alignment in expectations by prioritizing business critical assets.
    * Constraint maximum severity that can be set by the hacker is limited for the asset. (e.g., no alerts for a "Critical" vulnerability in your static marketing sites)
