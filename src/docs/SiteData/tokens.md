---
title: Tokens
layout: layouts/page.html
eleventyNavigation:
  key: Tokens
  order: '7'
tags: Site Data
draft: false
_schema: default
---
![](/assets/images/uploads/image-93.png)

Welcome to the token system for your website! Tokens are a powerful tool that allows you to dynamically update and reuse content across your website, saving time and ensuring consistency. This guide will explain what tokens are, how to use them, and provide practical examples and benefits.

---

## What Are Tokens?

Tokens are placeholders for data that can be inserted anywhere on your website. Instead of writing the same information multiple times across pages, you can use a token. When the token’s value is updated, the change will reflect wherever the token is used.

### Types of Tokens

1. **User-Generated Tokens (`[[tk.*]]`)**: These are custom tokens you create for specific needs, such as promotional messages or reusable text.
2. **Site Tokens (`[[st.*]]`)**: Predefined tokens linked to your site’s information, such as contact details, business name, or hours.
   1. **Available Site Tokens**
      1. **name**. Usage example: **`[[st.name]]`**
      2. **legalName**: Usage example: **`[[st.legalName]]`**
      3. **url**: Usage example **`[[st.url]]`**
      4. **contactInfo**:
         1. **email**: Usage example **`[[st.contactInfo.email]]`**
         2. **phone**: Usage example **`[[st.contactInfo.phone]]`**
         3. **location**: Usage example **`[[st.contactInfo.location]]`**
         4. **hours**: Usage example **`[[st.contactInfo.hours]]`**

![](/assets/images/uploads/image-89.png)

---

## How to Create Custom Tokens

Tokens and token groups as easily created your "Tokens" data file. You can create single tokens or token groups that can have singles or even more groups. Talk about tokenception.

![](/assets/images/uploads/image-90.png)

---

## Benefits of Using Tokens

* **Time-Saving**: Update content in one place and see it change everywhere.
* **Consistency**: Avoid mismatched or outdated information.
* **Scalability**: Ideal for frequently updated content like promotions or seasonal changes.

### When to Use Tokens

* **Use Tokens**:
  * For information that appears in multiple places (e.g., contact details).
  * For content that changes regularly (e.g., promotions).
* **Avoid Tokens**:
  * For static or rarely updated content (e.g., About Us page).
  * When the complexity of managing tokens outweighs the benefit.

---

## How to Use Tokens

### Syntax

Tokens follow a specific format depending on their type:

* **User-Generated Tokens**: `[[tk.key]]` or `[[tk.groupName.key]]`
* **Site Tokens**: `[[st.key]]` or `[[st.contactInfo.key]]`

### Examples of Token Usage in Text

* **Using a Single Token**: "For inquiries, email us at \[\[st.contactInfo.email\]\]."
* **Using a Token Group**: "Visit us at \[\[st.contactInfo.location\]\]. Call us at \[\[st.contactInfo.phone\]\]. We’re open \[\[st.contactInfo.hours\]\]."

&nbsp;

![](/assets/images/uploads/image-94.png)

---

## Common Use Cases

### **1\. Displaying Contact Information**

#### **Scenario**: You want your contact details to appear consistently across your website.

#### **Solution**:

Use the `st.contactInfo` tokens:

**Example Text:** "Feel free to reach out to us at \[\[st.contactInfo.email\]\] or call \[\[st.contactInfo.phone\]\]. You can visit our location at \[\[st.contactInfo.location\]\]. We’re open \[\[st.contactInfo.hours\]\]."

![](/assets/images/uploads/image-92.png)

**Outcome:** If your email or phone number changes, update it once in the token configuration, and the change applies everywhere.

### **2\. Promoting Special Offers**

#### **Scenario**: You want to highlight a seasonal discount across your site.

#### **Solution**:

Create a user-generated token:

**Example Token Definition:**

* `[[tk.promo.discount]]`: "Get 15% off all services until December 31st!"

![](/assets/images/uploads/image-85.png)

**Example Text:** "Don’t miss out on our latest deal: \[\[tk.promo.discount\]\]."

**Outcome:** Update the `[[tk.promo.discount]]` token when the promotion changes, and all mentions update automatically.

### **3\. Managing Team Information**

#### **Scenario**: Showcase team members on a "Meet Our Team" page or within service-related content.

#### **Solution**:

Use a token group for team information.

**Example Token Definition:**

* `[[tk.team.leadTechnician.name]]`: "John Doe"
* `[[tk.team.leadTechnician.title]]`: "Lead Technician"

![](/assets/images/uploads/image-86.png)

![](/assets/images/uploads/image-87.png)

![](/assets/images/uploads/image-88.png)

**Example Text:** "Our team is led by \[\[tk.team.leadTechnician.name\]\], our highly skilled \[\[tk.team.leadTechnician.title\]\]."

**Outcome:** Easily update team details in one place as staff changes.

---

## Advanced Usage

### Token Groups

Token groups allow you to organize related tokens under a single category for better management.

**Example:**

* Group: `contactInfo`
  * `[[st.contactInfo.email]]`: "[info@example.com]()"
  * `[[st.contactInfo.phone]]`: "123-456-7890"

Use these tokens anywhere on your site without duplicating information.

### Slugified Keys

To ensure tokens are compatible, complex keys are "slugified," meaning special characters are replaced with hyphens (`-`) and converted to lowercase. For example:

* User-defined key: `Sales/Contact Info`
* Usable token: `[[tk.sales-contact-info]]` or `[[tk.Sales/Contact Info]]`

Both forms are valid, allowing flexibility in how tokens are referenced.

---

## Tips for Managing Tokens

1. **Plan Your Tokens**: Identify reusable content before creating tokens.
2. **Use Descriptive Keys**: Choose clear, descriptive names for your tokens to avoid confusion.
3. **Test Before Updating**: Preview your site after updating tokens to ensure they display correctly.

---

## Summary

Tokens are a powerful way to manage content dynamically across your website. By using site tokens for common details like contact information and user-generated tokens for promotions or team details, you can ensure consistency and save time. While tokens are highly beneficial for frequently updated or reused content, they might be overkill for static information.

Start leveraging tokens today to simplify your website updates and create a seamless experience for your visitors!