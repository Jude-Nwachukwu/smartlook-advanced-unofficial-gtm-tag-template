# Smartlook Advanced Unofficial GTM Tag Template

This custom tag template for **Google Tag Manager (GTM)** allows you to implement **advanced Smartlook tracking** features without manually writing custom JavaScript code.

> Developed by **Jude Nwachukwu Onyejekwe** for [DumbData](https://dumbdata.co)  
> Licensed under the **Apache 2.0 License**

---

## ✅ Features

This GTM tag template supports:

- 🎯 **Event Tracking** – Track custom user interactions
- 👤 **User Identification** – Send user IDs and metadata
- 🎮 **Global Event Properties** – Attach persistent metadata to all Smartlook events
- 💻 **Custom Navigation Events** – Track virtual pageviews and dynamic URLs
- 🛑 **Custom Error Logging** – Report custom errors into Smartlook's console

---

## 🛠️ Installation

1. Open your GTM container.
2. Go to **Templates > Tag Templates > New**.
3. Click the **3-dot menu** in the top-right corner and choose **Import**.
4. Upload the `.tpl` file from this repository.
5. Save and name the template (e.g., `Smartlook Advanced Unofficial`).

---

## ⚙️ Configuration Instructions

When adding a new tag using this template, choose the **Tracking Tag Type** that best fits your use case:

---

### 🎯 Event Tracking

Track user interactions like button clicks, purchases, form submissions, etc.

**Required:**
- **Smartlook Event Name** – e.g., `Viewed Product`

**Optional:**
- **Add Smartlook Event Properties** – A table where you can add:
  - `Smartlook Property Key` (e.g., `productId`)
  - `Value` (e.g., `{{DLV - product_id}}`)

---

### 👤 User Identification

Identify users and attach user metadata.

**Required:**
- **Smartlook User ID** – Select a GTM variable that holds the user's unique ID.

**Optional:**
- **Add Additional User Metadata** – A table where you can define:
  - `Identifier Type` (e.g., Name, Email, Phone)
  - `Value` (e.g., `{{DLV - user_email}}`)

---

### 🎮 Global Event Properties

Add key-value metadata to **all** Smartlook events.

**Required:**
- **Add Smartlook Global Event Properties** – A table with:
  - `Property Key` (e.g., `plan`)
  - `Value` (e.g., `{{DLV - plan_type}}`)

---

### 💻 Custom Navigation Event

Track single-page app routing or virtual pageviews.

**Required:**
- **New Page URL** – Enter the full URL or a relative path (e.g., `/checkout-confirmation`)

---

### 🛑 Custom Error Tracking

Send handled or custom error messages into Smartlook.

**Required:**
- **Log Error Message** – A string or variable reference that describes the error (e.g., `Form submission failed`)

---

### ⚙️ Optional Configuration

**Optional:**
- **Disable Console Logging** – Check this to suppress logging output in the browser console.

---

## 🧾 License

This project is licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0).

---

## 🤝 Credits

Created with ❤️ by **Jude**  
For [DumbData](https://dumbdata.co)
