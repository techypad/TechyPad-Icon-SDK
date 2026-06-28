<div align="center">
  <img src="https://cdn.techypad.in/images/logo.png" alt="TechyPad Logo" width="200"/>
</div>

# 🎨 TechyPad Icon SDK & Repository

Welcome to the official **TechyPad Icon SDK** repository! This is the central hub where the community shares their custom designs to completely customize the TechyPad experience, and where creators can learn how to build their own packs.

---

## 📥 How to Install an Icon Pack
1. Browse the icon packs in this repository or on the community forums.
2. Download the `.techypadiconpack` file you want.
3. Open the TechyPad Desktop App.
4. Double-click the downloaded `.techypadiconpack` file (or drag and drop it into the app).
5. The app will automatically verify its security with our servers and install it!

---

## 🛠️ How to Create Your Own Icon Pack (SDK)

Icon packs allow you to completely customize the look of your TechyPad! By creating a custom icon pack, you can override the default icons of any plugin (like Discord, OBS, Premiere Pro, etc.) with your own designs.

Icon packs are designed to be extremely easy to create and share—**no coding or compiling required!**

### Step 1: Create the Folder
Create a new folder somewhere on your computer (e.g., `my_awesome_icons`). 

### Step 2: The `manifest.json` File
Inside that folder, create a file named `manifest.json`. This tells TechyPad about your pack. Use this template:

```json
{
  "id": "com.yourname.awesome_icons",
  "name": "My Awesome Icons",
  "version": "1.0.0",
  "author": "Your Name"
}
```
> [!IMPORTANT]
> Make sure the `id` is unique so it doesn't conflict with other icon packs!

### Step 3: Add Your Images
Create an `icons/` folder next to your `manifest.json`. Place all your `.png`, `.jpg`, or `.svg` files in this folder. 
When a user installs your pack, these icons will show up in the TechyPad Icon Library, allowing them to map your custom graphics to any button action!

> [!TIP]
> **Resolution:** We recommend using `144x144` pixel square images for the best clarity on the physical device.

---

## 📦 Packaging and Local Testing

Because Icon Packs are meant to be easily shared by creators everywhere, they are not compiled into DLLs. They are simply `.zip` files!

### 1. Zipping Your Pack
1. Open your `my_awesome_icons` folder so you can see `manifest.json` and the `icons/` folder.
2. Select **both** the `manifest.json` file and the `icons/` folder at the same time (e.g. press Ctrl+A).
3. Right-click on one of the highlighted items and compress them into a `.zip` file (e.g., `my_awesome_icons.zip`).

> [!WARNING]
> **Do not right-click the parent folder itself to zip it!** If you zip the parent folder, the `manifest.json` will be hidden inside a sub-folder and TechyPad will fail to read it. You must highlight the internal files directly and zip them together.

### 2. Test Locally (Developer Mode)
Before submitting, make sure it works! 
1. Open the TechyPad app and go to **Settings**.
2. Turn on **Developer Mode**.
3. You can now load your raw `.zip` file directly into the app to test how it looks on your device.

---

## 🚀 How to Submit Your Icon Pack

We love community creations! You cannot share your raw `.zip` file directly with users because standard TechyPad apps will reject them for security reasons. Instead, submit it to us!

Once you are happy with your icon pack and have tested it locally:
1. Go to **[submit.techypad.in](https://submit.techypad.in)** in your web browser.
2. Fill out the submission form with your name and pack details.
3. Upload your raw `.zip` file.
4. Our admin team will review your pack. If it meets our quality and security guidelines, we will cryptographically verify it, package it into a secure `.techypadiconpack` file, and publish it on our **[Marketplace](https://marketplace.techypad.in)**!

### 📜 Rules for Submission
- **No NSFW Content:** Keep it clean and family-friendly.
- **Copyright:** Do not steal icons from other artists without permission.
- **File Size:** Try to keep your images under 144x144 resolution so they load instantly on the hardware.
## 🧩 Complete the Experience

The Icon SDK works alongside the rest of the TechyPad developer ecosystem.

### 🔌 TechyPad Plugins SDK
Build plugins for TechyPad using the official SDK, APIs, examples, and documentation.

➡️ https://github.com/techypad/TechyPad-Plugins-SDK

---

### 🛠️ TechyPad Setup
Need to install TechyPad or prepare your development environment? Start here.

➡️ https://github.com/techypad/techy-pad-setup

---

✨ Great plugins deserve great icons. Use this SDK to keep every plugin looking clean, consistent, and unmistakably TechyPad.
