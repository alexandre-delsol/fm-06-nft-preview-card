# Frontend Mentor — NFT Preview Card Component

![Design preview for the NFT preview card component](./design/desktop-design.jpg)

## 📋 About

This project is my solution to the **[NFT Preview Card Component](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U)** challenge from Frontend Mentor.

The goal was to reproduce the provided design as accurately as possible while practicing HTML structure, CSS layout, responsive design, and hover interactions.

## 🚀 Built With

* HTML5
* CSS3
* CSS Custom Properties
* CSS Nesting
* Flexbox
* Responsive Design
* Git / GitHub

## 🎯 Features

* Responsive NFT preview card
* NFT image display
* Cyan overlay on image hover
* View icon displayed on image hover
* Hover effects on links
* NFT information display
* Creator information with avatar

## 🧠 What I Learned

This challenge helped me practice several important CSS concepts.

### Positioning

Using:

```css
position: relative;
position: absolute;
```

to position the view icon relative to the image container.

### Centering with `transform`

```css
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
```

This technique allows an absolutely positioned element to be centered within its parent.

### CSS `::after` pseudo-element

I used `::after` to create the cyan overlay without adding an additional HTML element.

```css
.image-container::after {
    content: "";
    position: absolute;
    inset: 0;
}
```

### CSS Nesting

Native CSS nesting was used to keep related styles grouped together.

```css
.image-container {
    &::after {
        /* ... */
    }

    &:hover {
        /* ... */
    }
}
```

### Flexbox

Flexbox was used to:

* center the card on the page;
* organize the card content vertically;
* align the NFT details;
* align the creator avatar and information.

## 📱 Responsive Design

The project was developed using a **mobile-first approach**.

The base styles target smaller screens, with media queries used only where the layout requires adjustments for larger screens.

## ♿ Accessibility

Some accessibility practices were used throughout the project:

* semantic HTML elements such as `<main>` and `<article>`;
* descriptive `alt` text for informative images;
* empty `alt` attributes for decorative images;
* `<a>` elements for interactive links.

## 🛠️ Getting Started

Clone the repository:

```bash
git clone https://github.com/alexandre-delsol/fm-06-nft-preview-card.git
```

Navigate to the project:

```bash
cd fm-06-nft-preview-card
```

Open `index.html` in your browser.

No additional dependencies or installation are required.

## 📚 Challenge

This challenge was provided by **Frontend Mentor**.

* [Frontend Mentor](https://www.frontendmentor.io/)
* [NFT Preview Card Component](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U)

## 👨‍💻 Author

**Alexandre DELSOL**

* GitHub: [alexandre-delsol](https://github.com/alexandre-delsol)
* Frontend Mentor: [@alexandre-delsol](https://www.frontendmentor.io/profile/alexandre-delsol)
