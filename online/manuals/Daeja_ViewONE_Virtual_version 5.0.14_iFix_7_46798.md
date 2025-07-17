
# Daeja_ViewONE_Virtual_version 5.0.14_iFix_7_46798

##### q: Daeja ViewONE Virtual version 5.0.14 iFix 7 (46798) how can i change the find result color marking inside the document

To change the **find result color marking** in IBM Daeja ViewONE Virtual version 5.0.14 iFix 7, you'll need to customize the viewer using its **HTML parameters or JavaScript API**, as the viewer is designed to be highly configurable.

### 🎨 How to Change Find Result Highlight Color

IBM Daeja ViewONE uses **search highlighting** to mark found text in documents. The color of this highlight is typically controlled via **HTML configuration parameters** or **JavaScript settings** in the viewer's initialization.

Here’s how you can approach it:

#### ✅ Option 1: Use HTML Parameters
You can set the highlight color using the `highlightColor` parameter in your viewer configuration.

```html
<param name="highlightColor" value="#FF0000"> <!-- Red highlight -->
```

- This parameter should be placed in the HTML that embeds the viewer.
- Use any valid hex color code (`#RRGGBB`) to customize the color.

#### ✅ Option 2: Use JavaScript API
If you're initializing the viewer via JavaScript, you can set the highlight color like this:

```javascript
viewONE.setHighlightColor("#00FF00"); // Green highlight
```

- This method allows dynamic control over the highlight color.
- You can call it after the viewer is initialized.

### 🛠 Additional Tips
- Make sure your viewer is configured to allow search and highlight features.
- Clear browser cache after making changes to ensure updates are reflected.
- Refer to the [IBM Daeja ViewONE 5.0.14 Developer’s Guide](https://www.ibm.com/support/pages/ibm-daeja-viewone-5014-release-notes) for deeper customization options.

Would you like help locating the exact configuration file or script in your setup?

-----

##### #2: Daeja ViewONE Virtual	version 5.0.14 iFix 7 (46798) how can i change the find result color marking inside the document

For **Daeja ViewONE Virtual version 5.0.14 iFix 7 (46798)**, changing the color of the **find result highlighting** inside the document typically involves modifying the viewer’s configuration settings or stylesheets, since the find result colors are controlled either by the viewer's configuration files or sometimes via CSS if the viewer supports that.

Here’s a general approach to customize the find result highlight color:

### 1. Check Viewer Configuration Files

* Daeja ViewONE Virtual uses XML-based configuration files to control many aspects of the viewer’s behavior and appearance.
* Look for a configuration file such as `ViewONEConfig.xml` or a similar config file that the viewer uses.
* Inside this config, there might be settings related to search or find highlight colors.

### 2. Look for Highlight Color Settings

* Search for keywords like `"highlight"`, `"find"`, `"search"`, `"selection"`, or `"color"` in the config files.
* Often the color will be specified in a hex code format (e.g., `#FF0000` for red).

Example snippet might look like:

```xml
<FindHighlightColor>#FFFF00</FindHighlightColor>
```

If you find such a setting, change the hex color to your preferred highlight color.

### 3. CSS or Style Sheets (if applicable)

* Some Daeja ViewONE Virtual installations allow overriding the viewer's styles via CSS.
* If you have access to the CSS files or style overrides, search for classes like `.find-result`, `.highlight`, or similar.
* Change the CSS color or background-color for the highlight.

Example CSS:

```css
.find-result {
  background-color: #00FF00 !important; /* bright green */
}
```

### 4. Viewer API or JavaScript (if applicable)

* If the viewer is embedded in a web page, sometimes you can override find highlight colors via JavaScript APIs or initialization options.
* Check the Daeja developer or user documentation for any such API.

---

### If you don't have direct access to config files:

* Sometimes find highlight color is fixed or not user-changeable via GUI.
* You may need to contact Daeja support or check official documentation for customization options in your specific build.

---

### Summary for your version:

* Locate the **configuration XML file** for your viewer.
* Search for find/search highlight color settings.
* Edit the color value (hex code).
* Restart or reload the viewer for changes to take effect.
  
-----

##### #3: Daeja ViewONE Virtual	version 5.0.14 iFix 7 (46798) command manual


IBM Daeja ViewONE Virtual version 5.0.14 iFix 7 (46798) does not provide a dedicated command-line manual. However, you can utilize the following resources and methods to configure and customize the viewer:

---

### 🔧 Configuration and Customization Resources

1. **HTML Parameters and JavaScript API**: Daeja ViewONE Virtual offers a rich toolkit for integration and customization using HTML parameters and JavaScript API methods. For detailed information, refer to the [IBM Daeja ViewONE 4.1.5 Virtual Developer's Guide](https://delivery04.dhe.ibm.com/sar/CMA/OSA/08je1/0/5.0.6_DAEJA_VIEWONE_IFIX007_Readme.htm).

2. **Release Notes and Readme Files**: The release notes and readme files for Daeja ViewONE Virtual version 5.0.14 iFix 7 provide information about new features, fixes, and known problems. You can access them here:

   * [IBM Daeja ViewONE 5.0.14 iFix 7 Readme](https://download4.boulder.ibm.com/sar/CMA/OSA/0cpn6/1/5.0.14_DAEJA_VIEWONE_IFIX007_Readme.htm)
   * [IBM Daeja ViewONE 5.0.14 Release Notes](https://www.ibm.com/support/pages/ibm-daeja-viewone-5014-release-notes)&#x20;

3. **Installation and Deployment**: For installation instructions and deployment guidelines, refer to the [IBM Daeja ViewONE 5.0.14 Readme](https://delivery04.dhe.ibm.com/sar/CMA/OSA/0bw93/0/DAEJA_VIEWONE_5.0.14_Readme.htm).

---

### 🛠️ Customizing Find Result Highlight Color

To customize the find result highlight color within the document viewer, you can modify the viewer's configuration files or stylesheets. Look for settings related to search or find highlight colors in the configuration files, and adjust the color values as needed.

---

### 📞 Seeking Further Assistance

If you require more detailed information or specific guidance, consider reaching out to IBM Support or consulting the official [IBM Daeja ViewONE Knowledge Center](https://www.ibm.com/support/pages/ibm-daeja-viewone-virtual-version-501-release-notes) for comprehensive documentation and resources.


---

If you want, I can help you with a more specific search or example based on the config files you have. Do you have access to any of the configuration files or can you share a snippet?

-----
