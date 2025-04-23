# Cockpit Store

Welcome to the Cockpit Store repository – a centralized JSON-powered showcase for all your Cockpit Panel rebrands, modules, and offerings.

## 🎯 Purpose

This repo provides a flexible way for resellers, developers, and hosting providers to share their available Cockpit Panel modules and IPTV apps with clients via a JSON file.

---

## 🛠 How to Use

1. **Clone this repository:**
   ```
   git clone https://github.com/Cockpit-Panel/cockpit-store.git
   ```

2. **Edit the `api.json` file** to add your own rebranded panels, modules, or applications.

   Each product entry supports:
   - `name`, `description`
   - Price fields (`hosted`, `selfhosted`, `sourcecode`) and their discounted `*_offer` versions
   - `main_image`, additional `images[]`
   - Optional: `purchase` URL, `ytvideo`, and `telegram` contact

   Example:
   ```json
   {
     "name": "Cockpit Panel: Your Custom Module",
     "description": "Your description here...",
     "hosted": "100.00",
     "hosted_offer": "80.00",
     "selfhosted": "200.00",
     "selfhosted_offer": "150.00",
     "sourcecode": "300.00",
     "sourcecode_offer": "250.00",
     "main_image": "https://your-image-url.com/main.png",
     "images": [
       "https://your-image-url.com/1.png",
       "https://your-image-url.com/2.png"
     ],
     "ytvideo": "https://youtube.com/your-demo",
     "telegram": "https://t.me/yourcontact",
     "purchase": "https://your-store.com/product-link"
   }
   ```

3. **Commit your changes:**
   ```
   git add api.json
   git commit -m "Add my rebranded modules"
   git push
   ```

---

## 💡 Use Case

This setup is perfect for:
- Freelancers offering rebranded applications Cockpit Panels
- Sellers managing hosted/self-hosted rebrands
---

## ✅ Tips

- Leave unused fields (like `ytvideo`, `sourcecode`, or `images`) empty ("") if not applicable.
- Keep your JSON valid! Use a [JSON validator](https://jsonlint.com/) if needed.
- Make sure image URLs and links are accessible and direct.

---

## 🔗 Useful Links

- [Official Store](https://store.cockpit.lol)
- [Telegram Contact](https://t.me/ianwoneill)
- [Cockpit Panel Docs](https://store.cockpit.lol/knowledgebase.php)

---

Feel free to fork this repo and make it your own. The goal is flexibility, transparency, and easy integration.
