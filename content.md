## Gallery

#gallery-section {
/_background: url('/images/pattern/pattern04.jpg')repeat fixed;_/
}

#gallery.d-grid {
display: grid;
grid-template-columns: repeat(7, 1fr);
grid-auto-rows: 220px;
grid-gap: 7px;
grid-template-areas: "one one one two two two two" "one one one three three four four";
}

.gallery-item {
position: relative;
}

    .gallery-item:nth-child(1) {
        grid-area: one;
    }

    .gallery-item:nth-child(2) {
        grid-area: two;
        margin: 0;
    }

    .gallery-item:nth-child(3) {
        grid-area: three;
    }

    .gallery-item:nth-child(4) {
        grid-area: four;
    }

    .gallery-item a {
        position: absolute;
        left: 0;
        right: 0;
        bottom: 0;
        top: 0;
        overflow: hidden;
    }

    .gallery-item img {
        height: 100%;
        width: 100%;
        object-fit: cover;
    }

---
