# 🌌 Mission: The Jovian Drift SOS

## 📋 Objective

Construct the emergency transmission interface for the shuttle Europa-1.
You are currently in orbit around Jupiter, and your only hope is to send a
high-priority distress signal to Earth.

---

## 📁 Getting Started

1. Create a new file called `index.html` in the root of this project ( don't nest it in folders like tsotne/index.html or khatia/index.html) ✅
2. Start with the basic HTML5 document structure including:
   - A DOCTYPE declaration at the very top
   - An `<html>` element with the `lang` attribute set to "en" ✅
   - A `<head>` section containing:
     - A `<meta>` tag for character encoding (UTF-8)✅
     - A `<meta>` tag for viewport settings (responsive design) ✅
     - A `<title>` element with the text "Jovian Drift SOS" ✅
   - A `<body>` section where all your visible content will go ✅

---

## 🛠️ Instructions for Students

### Phase 1: The Transmission Protocol (The Form)

The signal contains sensitive biometric and mission data, so it must be sent securely.

- Create a `<form>` element inside the `<body>` tag ✅
- Set the `method` attribute to "post" (this determines how the form data is sent. "post" is one of several HTTP methods available, but we only need this one for now. If you're curious about other HTTP methods, feel free to research them, but we'll explain them in detail in future lessons.) ✅
- Set the `action` attribute to "#" (the `action` attribute tells the form where to send the data when it's submitted. In this exercise, we're using "#" which is a special value that means "stay on the current page" - this simulates sending the transmission to the ship's computer without actually leaving the page. In real websites, the action would point to a server URL that processes the form data.) ✅
- All subsequent fieldsets and input elements should be nested inside this form element

---

### Phase 2: Pilot Credentials (Fieldset 1)

Earth needs to know who is sending the message.

1. Create a `<fieldset>` with a `<legend>` titled **"Pilot Credentials"**✅

2. **Pilot Name:**

   - Create a `<label>` element with the text "Pilot Name:" ✅
   - Give the label a `for` attribute with a unique value (like "pilot-name")✅
   - Create an `<input>` element with `type` attribute set to "text" ✅
   - Give the input an `id` attribute that matches the label's `for` value ✅
   - Add a `name` attribute to the input (use something like "pilot_name")✅
   - Add the `required` attribute (boolean attribute, no value needed) ✅
   - Add a `placeholder` attribute with the value "Enter name"✅

3. **Access Code:**

   - Create a `<label>` element with the text "Access Code:" ✅
   - Give it a `for` attribute with a unique identifier✅ (setted access-code)
   - Create an `<input>` element with `type` attribute set to "password"
   - Connect it to the label using a matching `id` attribute✅
   - Add a `name` attribute (like "access_code")✅
   - Add the `required` attribute✅

4. **Command Email:**
   - Create a `<label>` element with the text "Command Email:"✅
   - Give it a `for` attribute with a unique identifier✅
   - Create an `<input>` element with `type` attribute set to "email"✅
   - Connect it to the label using a matching `id` attribute✅
   - Add a `name` attribute (like "email")✅
   - Add the `required` attribute✅

---

### Phase 3: Vessel Diagnostics (Fieldset 2)

The rescue team needs to know the state of your ship.

1. Create a `<fieldset>` with a `<legend>` titled **"Vessel Diagnostics"**✅

2. **Hull Damage:**

   - Create a `<label>` element with the text "Hull Damage (%):"✅
   - Give it a `for` attribute with a unique identifier✅
   - Create an `<input>` element with `type` attribute set to "number"✅
   - Connect it to the label using a matching `id` attribute✅
   - Add a `name` attribute (like "hull_damage")✅
   - Add the `required` attribute✅

3. **Emergency Level:**
   - Create a `<label>` element with the text "Emergency Level:"✅
   - Give it a `for` attribute with a unique identifier✅
   - Create a `<select>` element (this creates a dropdown menu)✅
   - Connect it to the label using a matching `id` attribute✅
   - Add a `name` attribute to the select element✅
   - Add the `required` attribute to the select element✅
   - Inside the select element, nest three `<option>` elements✅
   - Each option should have a `value` attribute (like "low", "medium", "high")✅
   - Each option's text content should be: "Low", "Medium", and "High" respectively✅

---

### Phase 4: Mission Log & Evidence (Fieldset 3)

Explain the situation and agree to safety protocols.

1. Create a `<fieldset>` with a `<legend>` titled **"Mission Log & Evidence"**✅

2. **SOS Message:**

   - Create a `<label>` element with the text "SOS Message:"✅
   - Give it a `for` attribute with a unique identifier✅
   - Create a `<textarea>` element (note: this is NOT an input element)
   - Connect it to the label using a matching `id` attribute✅
   - Add a `name` attribute to the textarea✅
   - Add the `required` attribute to the textarea✅
   - Add a `rows` attribute with the value "3" (this sets the visible height)✅

3. **Quarantine Agreement:**
   - Create a `<div>` element as a container wrapper ✅
   - Inside the div, create an `<input>` element with `type` attribute set to "checkbox" ✅
   - Give the checkbox an `id` attribute (like "quarantine") ✅
   - Add a `name` attribute to the checkbox ✅
   - Add the `required` attribute to the checkbox
   - After the input, create a `<label>` element with text "I agree to quarantine protocols."✅
   - Connect the label to the checkbox by setting the label's `for` attribute to match the checkbox's `id`✅

---

### Phase 5: The Control Panel (Buttons)

Your code is only valid if you can send it!

- Create a `<button>` element with a `type` attribute set to "submit" ✅
- The button's text content should be: "INITIATE TRANSMISSION" ✅
- Create a second `<button>` element with a `type` attribute set to "reset" ✅
- The button's text content should be: "RESET SYSTEM" ✅
- Place both buttons inside the form, typically after all fieldsets ✅

---

## ✅ Checklist for Success

Before adding the WOW effect, verify:

- [ ] **Label IDs:** Does every `<label>` have a `for` attribute that matches the `id` of its input/select/textarea?
- [ ] **Required Fields:** Did you add the `required` attribute to every input, select, and textarea to prevent empty transmissions?
- [ ] **Semantic Structure:** Did you use `<fieldset>` and `<legend>` for all three sections (Pilot Credentials, Vessel Diagnostics, Mission Log)?
- [ ] **Types:** Did you use the correct input types?
  - `type="text"` for Pilot Name
  - `type="password"` for Access Code
  - `type="email"` for Command Email
  - `type="number"` for Hull Damage
  - `type="checkbox"` for Quarantine Agreement
- [ ] **Names:** Did you add a `name` attribute to all form controls?
- [ ] **Form Works:** Can you fill out and submit the form without errors?

---

## 🎨 FINAL: WOW Effect

We know about the WOW effect :)

Once your form is complete and working, add these final touches:

**Step 1: Add the CSS stylesheet link**

- In the `<head>` section, find the `<title>` element
- Right AFTER the `</title>` closing tag, add this exact code:
  ```html
  <link rel="stylesheet" href="./styles/styles.css" />
  ```
- Your code should look like this:
  ```html
      <title>Jovian Drift SOS</title>
      <link rel="stylesheet" href="./styles/styles.css">
  </head>
  ```

**Step 2: Add the animated background iframe**

- In the `<body>` section, find your opening `<form>` tag
- Right BEFORE the `<form>` tag, add this exact code:
  ```html
  <iframe id="bg-frame" src="./styles/effect.html"></iframe>
  ```
- Your code should look like this:

  ```html
  <body>
    <iframe id="bg-frame" src="./styles/effect.html"></iframe>

    <form method="post" action="#"></form>
  </body>
  ```

**Step 3: Add the launch control script**

- In the `<body>` section, find the closing `</body>` tag (it should be the very last line of your HTML)
- Right BEFORE the `</body>` tag, add this exact code:
  ```html
  <script src="./scripts/launch.js"></script>
  ```
- This script enables the interactive launch sequence when you submit the form
- Your code should look like this at the end:

  ```html
      </form>

      <script src="./scripts/launch.js"></script>
  </body>
  </html>
  ```

**Important Notes:**

- The CSS link must be in the `<head>` section (where all stylesheets go)
- The iframe must be in the `<body>` section (only visible content goes here)
- Make sure the iframe comes BEFORE your form in the body
- The script must be placed at the END of the `<body>` section, right before the closing `</body>` tag (after your closing `</form>` tag)

🎉 **Congratulations!** Your transmission interface is now operational with a stunning Jupiter background and an interactive launch sequence!
