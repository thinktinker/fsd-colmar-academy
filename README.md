# 🌐 Colmar Academy Webpage Project

This project guides you through the process of creating a **responsive webpage**. You’ll work across three branches, each focusing on a different aspect of front-end development:

**Branches**

1. **main:** Setting up the Skeleton
2. **desktop-mode:** Creating the Desktop Design
3. **responsive-mode:** Creating the Responsive Design

## 🖥️ 1. Setting Up the Skeleton

### 🎯 Objectives

- In this branch, you will **set up the foundational structure** of the webpage using **semantic HTML5 elements**.
- No CSS styling will be added yet — the focus is on creating a **well-organized and meaningful HTML layout**.

---

### 🗂️ Files Involved

- `index.html`

---

### 🛠 Tasks

You will:

1. Create the base structure of the webpage with semantic HTML.
2. Include placeholder comments (`<!-- TODO -->`) for future sections.
3. Organize the layout into clear, meaningful sections.

---

### 🔑 Key HTML Concepts Introduced

| Concept                                                                  | Description                                                |
| ------------------------------------------------------------------------ | ---------------------------------------------------------- |
| `<!DOCTYPE html>`                                                        | Declares the document as HTML5.                            |
| `<html lang="en">`                                                       | Defines the language of the page.                          |
| `<meta charset="UTF-8">`                                                 | Ensures the webpage displays special characters correctly. |
| `<meta name="viewport" content="width=device-width, initial-scale=1.0">` | Makes your site mobile-friendly.                           |
| `<head>`                                                                 | Contains metadata such as the title and stylesheet links.  |
| `<body>`                                                                 | Contains all visible webpage content.                      |
| Semantic tags (`<header>`, `<nav>`, `<section>`, `<footer>`)             | Provide structure and meaning to the page layout.          |
| Comments (`<!-- -->`)                                                    | Help mark unfinished sections and guide development.       |

---

### Basic Page Layout

Your HTML structure will include these main sections:

| Section      | Purpose                                             |
| ------------ | --------------------------------------------------- |
| **Navbar**   | Displays the logo and navigation menu.              |
| **Header**   | Introduces the academy and features a banner.       |
| **Practice** | Describes continuous learning and self-improvement. |
| **Events**   | Lists key activities and updates.                   |
| **Learning** | (Placeholder) For showcasing programs and lessons.  |
| **Thesis**   | (Placeholder) For featuring projects or research.   |
| **Footer**   | Displays copyright and policies.                    |

---

### Example Skeleton Structure

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <!-- TODO -->
    <!-- The meta tag sets the page's viewport to be mobile-friendly -->

    <title>Colmar Academy</title>
    <!-- TODO -->
    <!-- Incorporate external css styles here -->
  </head>

  <body>
    <!-- 1. Start of Navbar -->
    <nav>
      <!--  TODO: Add logo and navigation menu -->
    </nav>
    <!-- End of Navbar -->

    <!-- 2.  Start of header -->
    <header>
      <!-- TODO: Add hero image and welcome text -->
    </header>
    <!-- End of header -->

    <!-- 3. Start of practice -->
    <section id="practice">
      <!-- TODO: Add practice description -->
    </section>
    <!-- End of practice -->

    <!-- 3.1. Start of events -->
    <section id="events">
      <!-- TODO: Add events list -->
    </section>
    <!-- End of events -->

    <!-- 4. Start of learning -->
    <section id="learning">
      <!-- TODO: Add learning highlights -->
    </section>
    <!-- End of learning -->

    <!-- 5. Start of thesis -->
    <section id="thesis">
      <!-- TODO: Add featured project -->
    </section>
    <!-- End of thesis -->

    <!-- 6. Start of footer -->
    <footer>
      <!-- TODO: Add footer links and info -->
    </footer>
    <!-- End of footer -->
  </body>
</html>
```

---

## 🖥️ 2. Creating the Desktop Design

### 🎯 Objectives

- In this branch, you will **transform the HTML skeleton into a desktop-ready webpage** using HTML + CSS.
- You will apply layout techniques like **Flexbox** and **Grid**, add visual hierarchy, and style the main sections for large screens.

---

### 🗂️ Files Involved

- `index.html`
- `styles/styles.css`

---

### 🛠 Tasks

You will:

1. Link your HTML to the external CSS file (`styles.css`).
2. Add the **meta viewport tag** for mobile support.
3. Implement the sections: **Navbar**, **Header**, **Practice**, **Events**, and **Footer**.
4. Use **Flexbox** for alignment and **Grid** for page layout.
5. Apply color, typography, and spacing for a professional desktop appearance.

### 🔑 Key Styling Concepts

| Concept          | Description                                            |
| ---------------- | ------------------------------------------------------ |
| **CSS Reset**    | Removes browser default margins and paddings.          |
| **Flexbox**      | Aligns and distributes elements along a single axis.   |
| **CSS Grid**     | Provides control over overall page structure.          |
| **Typography**   | Controls text size, weight, and color for readability. |
| **Hover states** | Improve interactivity for links and buttons.           |

### 📄 Page Sections

#### ☑️ Navbar

- Uses Flexbox for horizontal alignment.
- Displays logo (`ic-logo.svg`) and navigation links.
- “Colmar” is bold; “Academy” is light for contrast.

```html
<!-- TODO -->
<!-- 1. Start of Navbar -->
<nav>
  <a href="#">
    <img
      class="logo"
      src="assets/images/ic-logo.svg"
      alt="Colmar Academy Logo"
    />
    <span class="logoname logoname-bold">Colmar</span>
    <span class="logoname logoname-light">Academy</span>
  </a>
  <ul>
    <li><a href="#">Our Campus</a></li>
    <li><a href="#">Online</a></li>
    <li><a href="#">Our Companies</a></li>
    <li><a href="#">Sign-in</a></li>
  </ul>
</nav>
<!-- End of Navbar -->
```

#### ☑️ Header

- Features a banner image and a textual call-to-action.
- The `Start here` button is styled to stand out.

```html
<!-- TODO -->
<!-- 2.  Start of header -->
<header class="imgcontainer">
    <img src="assets/images/banner.jpg" alt="Homepage Banner">
</header>

<header>
    <div>
        <h1>
            Learn something new everyday
        </h1>
        <h2>
            Lorem ipsum dolor sit amet consectetur adipisicing elit.
        </h2>
        <a href="">
            Start here
        </a>
    </div>
</header>
<!-- End of header -->
```

#### ☑️ Practice Section

- Combines an image and motivational text using Flexbox.
- Includes a highlighted quote by “Emmanuel, Sr Strategist at Hiring.com”.

```html
<!-- TODO -->
<!-- 3. Start of practice -->
<section class="practice">
    <div class="imgcontainer">
        <img src="assets/images/information-main.jpg" alt="Practice Banner">
    </div>
    <div class="practice-text">
        <h1>It doesn't hurt to keep practicing</h1>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Commodi dolores soluta nemo veritatis repellat deleniti autem itaque asperiores alias cumque? Inventore amet perferendis dicta iste eveniet perspiciatis atque delectus dolorem.<span>Emmanuel, Sr Strategist at Hiring.com</span>
        </p>
    </div>
</section>
<!-- End of practice -->
```

#### ☑️ Events Section

- Displays three events with image, title, and link.
- Uses a two-column grid layout for clean alignment.

```html
<!-- TODO -->
<!-- 3.1. Start of events -->
<section class="events">
    
    <div class="events-block">

        <img src="assets/images/information-orientation.jpg" alt="Event Orientation Image">

        <div class="events-text">
            <h3>Orientation Date</h3>
            <p>Tue 10/11 & Wed 10/12 8am-3pm</p>
            <a href="">Read More</a>
        </div>
    </div>
    
    <div class="events-block">
        
        <img src="assets/images/information-campus.jpg" alt="Event Orientation Image">
        
        <div class="events-text">
            <h3>Our Campus</h3>
            <p>Find which campus is close to you</p>
            <a href="">Read More</a>
        </div>

    </div>

    <div class="events-block">
        
        <img src="assets/images/information-guest-lecture.jpg" alt="Event Orientation Image">
        
        <div class="events-text">
            <h3>Our Guest Lecture</h3>
            <p>Join a keynote with Oliver Sack about music in medical treatment</p>
            <a href="#">Read More</a>
        </div>

    </div>
</section>
<!-- End of events -->
```

#### ☑️ Footer

- Contains copyright.
- Displays links for **Terms** and **Privacy Policy**.

```html
<!-- TODO -->
<!-- 6. Start of footer -->
<footer>
    <p>&copy; 2024 Colmar Academy. All rights reserved.</p>
    <ul>
        <li><a href="#">Terms</a></li>
        <li><a href="#">Privacy</a></li>
    </ul>
</footer>
<!-- End of footer -->
```

### ✅ Expected Outcome

A polished **desktop layout** of the landing page for Colmar Academy.  
Responsiveness will be handled in **Branch 3**.

---

## 🖥️ 3. Creating the Responsive Mode

### 🎯 Objective

In this branch, you’ll make the webpage **responsive** — adapting its layout to work seamlessly on **mobile and tablet screens**.  
You’ll use **CSS media queries** to adjust layout, visibility, and spacing for smaller viewports.

### 🗂️ Files Involved

- `index.html`
- `styles/styles.css`

---

### 🛠 Tasks

You will:

1. Add a **mobile navigation bar** (`#nav-mobile`) that displays only on smaller screens.
2. Create **mobile-specific images** for the Events section.
3. Use **media queries** to:
   - Hide or show elements based on screen width.
   - Adjust Flexbox and Grid layouts for vertical stacking.
   - Resize text and spacing for readability.
4. Ensure that sections like **Practice** and **Footer** look clean and accessible on mobile devices.

---

### 📱 Key Concepts in Responsive Design

| Concept                 | Description                                                                    |
| ----------------------- | ------------------------------------------------------------------------------ |
| **Meta viewport tag**   | Tells browsers to control layout based on device width.                        |
| **Media queries**       | CSS rules that apply only within specified screen width ranges.                |
| **Flexible images**     | Using `max-width: 100%` and `height: auto` to prevent overflow.                |
| **Visibility toggling** | Showing/hiding elements (`display: none` / `display: block`) for mobile views. |

---

### ⚙️ Implementation Walkthrough

#### 🧭 Mobile Navbar

```html
<nav id="nav-mobile">
  <a href="#">
    <img src="assets/images/ic-logo.svg" alt="Mobile Logo Home" />
  </a>
  <a href="#">
    <img src="assets/images/ic-on-campus.svg" alt="Mobile Logo Campus"/>
  </a>
  <a href="#"
    ><img src="assets/images/ic-online.svg" alt="Mobile Logo Online"/>
  </a>
  <a href="#">
    <img src="assets/images/ic-login.svg" alt="Mobile Logo Login"/>
  </a>
</nav>
```
