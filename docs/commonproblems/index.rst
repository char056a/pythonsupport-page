.. _commonproblems:

Common Problems
=================

Here you will find fixes for common problems related to Python, Conda, packages, environments and VS Code

.. card-carousel:: 3
    
    .. card:: Python
        :img-background: images/python_logo_TR.png
        :link: python
        :link-type: doc

        Fixes for common problems related to Python

    .. card:: Conda
        :img-background: images/conda_logo_TR.png
        :link: conda
        :link-type: doc

        Common problems related to conda, environments and packages

    .. card:: VS Code
        :img-background: images/VSC_logo_TR.png
        :link: vscode
        :link-type: doc

        Common problems related to Visual Studio Code


.. raw:: html

    <div class="container mt-5">
    <h2 class="text-center">Manual Card Carousel with Infinite Looping</h2>
    <div id="cardCarousel" class="carousel">
        <div class="carousel-inner" style="display: flex; overflow-x: auto; white-space: nowrap; scrollbar-width: none; -ms-overflow-style: none; transition: none;">
            <!-- Card 1 -->
            <a href="conda.html" class="card" style="flex: 0 0 auto; width: 100px; margin-right: 15px;">
                <div class="card-body">
                    <img src="C:\Users\charl\OneDrive\Dokumenter\pythonsupport-page\docs\commonproblems\images\conda_logo_tr.png" alt="Card Image" style="width: 100%; height: 100px; border-radius: 4px;">
                    <h5 class="card-title">Card 1</h5>
                    <p class="card-text">Content for Card 1.</p>
                </div>
            </a>
            <!-- Card 2 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <img src="C:\Users\charl\OneDrive\Dokumenter\pythonsupport-page\docs\commonproblems\images\conda_logo_tr.png" alt="Card Image" style="width: 100%; height: 100px; border-radius: 4px;">
                    <h5 class="card-title">Card 2</h5>
                    <p class="card-text">Content for Card 2.</p>
                </div>
            </div>
            <!-- Card 3 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <h5 class="card-title">Card 3</h5>
                    <p class="card-text">Content for Card 3.</p>
                </div>
            </div>
            <!-- Card 4 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <h5 class="card-title">Card 4</h5>
                    <p class="card-text">Content for Card 4.</p>
                </div>
            </div>
            <!-- Card 5 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <h5 class="card-title">Card 5</h5>
                    <p class="card-text">Content for Card 5.</p>
                </div>
            </div>
            <!-- Card 6 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <h5 class="card-title">Card 6</h5>
                    <p class="card-text">Content for Card 6.</p>
                </div>
            </div>
        </div>
    </div>

    <script>
        const carouselInner = document.querySelector('.carousel-inner');
        const cardWidth = 250 + 15; // Width of each card including margin
        let cardCount = document.querySelectorAll('.carousel-inner .card').length;

        // Function to duplicate the cards to create infinite loop effect
        function cloneCards() {
            const cards = Array.from(document.querySelectorAll('.carousel-inner .card'));
            // Clone the first 3 cards and append to the end
            for (let i = 0; i < 3; i++) {
                carouselInner.appendChild(cards[i].cloneNode(true));
            }
            // Clone the last 3 cards and prepend to the beginning
            for (let i = cardCount - 3; i < cardCount; i++) {
                carouselInner.insertBefore(cards[i].cloneNode(true), carouselInner.firstChild);
            }
        }

        // Wait for the page layout to render, then clone the cards
        window.addEventListener('load', () => {
            // Clone cards to create the infinite loop
            cloneCards();
            
            // Initially set scroll position to the first real card
            carouselInner.scrollLeft = cardWidth * 3;
        });

        // Function to handle infinite scrolling without jumping
        function handleInfiniteScroll() {
            const maxScrollLeft = carouselInner.scrollWidth - carouselInner.clientWidth;
            const currentScrollLeft = carouselInner.scrollLeft;

            // If the user has reached the end (last real card), reset scroll position to first card
            if (currentScrollLeft >= maxScrollLeft - cardWidth) {
                carouselInner.scrollLeft = cardWidth * 3;
            }

            // If the user has reached the start (first real card), reset scroll position to last card
            if (currentScrollLeft <= 0) {
                carouselInner.scrollLeft = cardWidth * (cardCount + 2);
            }
        }

        // Enable smooth scrolling without automatic jumping
        carouselInner.addEventListener('scroll', handleInfiniteScroll);

        // Enable mouse wheel scrolling
        carouselInner.addEventListener('wheel', (event) => {
            if (event.deltaY !== 0) {
                event.preventDefault();
                const scrollSpeed = 2.5; // Adjust multiplier for sensitivity
                carouselInner.scrollLeft += event.deltaY * scrollSpeed;
            }
        });
    </script>

    <style>
        /* Hide the default scrollbar for a cleaner look */
        .carousel-inner {
            scrollbar-width: none; /* For Firefox */
        }

        .carousel-inner::-webkit-scrollbar {
            display: none; /* For Chrome, Safari, and Edge */
        }
    </style>
    </div>


.. raw:: html

    <div class="container mt-5">
    <h2 class="text-center">Manual Card Carousel with Infinite Looping</h2>
    <div id="cardCarousel" class="carousel">
        <div class="carousel-inner" style="display: flex; overflow-x: auto; white-space: nowrap; scrollbar-width: none; -ms-overflow-style: none;">
            <!-- Card 1 -->
            <a href="document1.html" class="card-link" style="text-decoration: none; color: inherit; flex: 0 0 auto; margin-right: 15px;">
                <div class="card" style="width: 250px;">
                    <div class="card-body">
                        <h5 class="card-title">Card 1</h5>
                        <p class="card-text">Content for Card 1.</p>
                    </div>
                </div>
            </a>
            <!-- Card 2 -->
            <a href="document2.html" class="card-link" style="text-decoration: none; color: inherit; flex: 0 0 auto; margin-right: 15px;">
                <div class="card" style="width: 250px;">
                    <div class="card-body">
                        <h5 class="card-title">Card 2</h5>
                        <p class="card-text">Content for Card 2.</p>
                    </div>
                </div>
            </a>
            <!-- Card 3 -->
            <a href="document3.html" class="card-link" style="text-decoration: none; color: inherit; flex: 0 0 auto; margin-right: 15px;">
                <div class="card" style="width: 250px;">
                    <div class="card-body">
                        <h5 class="card-title">Card 3</h5>
                        <p class="card-text">Content for Card 3.</p>
                    </div>
                </div>
            </a>
        </div>
    </div>

    <script>
        const carouselInner = document.querySelector('.carousel-inner');
        const cardWidth = 250 + 15; // Card width including margin
        let originalCards = Array.from(carouselInner.children); // Store the original cards
        const totalRealCards = originalCards.length;
        let isInitialized = false;

        // Clone cards for infinite scrolling
        function setupInfiniteScroll() {
            if (isInitialized) return; // Prevent multiple initializations
            isInitialized = true;

            const fragmentStart = document.createDocumentFragment();
            const fragmentEnd = document.createDocumentFragment();

            // Clone the cards for both ends
            originalCards.forEach(card => {
                fragmentEnd.appendChild(card.cloneNode(true));
                fragmentStart.appendChild(card.cloneNode(true));
            });

            // Append and prepend clones
            carouselInner.appendChild(fragmentEnd);
            carouselInner.prepend(fragmentStart);

            // Set initial scroll position to the first real card set
            carouselInner.scrollLeft = cardWidth * totalRealCards;
        }

        // Maintain infinite scrolling logic
        function handleInfiniteScroll() {
            const maxScrollLeft = carouselInner.scrollWidth - carouselInner.clientWidth;
            const currentScrollLeft = carouselInner.scrollLeft;

            // Reset to start if scrolled past the end
            if (currentScrollLeft >= maxScrollLeft - cardWidth * totalRealCards) {
                carouselInner.scrollLeft = cardWidth * totalRealCards;
            }

            // Reset to end if scrolled past the start
            if (currentScrollLeft <= cardWidth * (totalRealCards - 1)) {
                carouselInner.scrollLeft = maxScrollLeft - cardWidth * (totalRealCards * 2);
            }
        }

        // Initialize the infinite scroll on page load
        window.addEventListener('load', () => {
            setupInfiniteScroll();
        });

        // Attach the scroll event to handle seamless looping
        carouselInner.addEventListener('scroll', handleInfiniteScroll);

        // Enable smooth mouse wheel scrolling
        carouselInner.addEventListener('wheel', (event) => {
            event.preventDefault();
            const scrollSpeed = 2.5; // Adjust sensitivity
            carouselInner.scrollLeft += event.deltaY * scrollSpeed;
        });
    </script>

    <style>
        /* Hide scrollbar for a clean look */
        .carousel-inner {
            scrollbar-width: none; /* Firefox */
        }

        .carousel-inner::-webkit-scrollbar {
            display: none; /* Chrome, Safari, Edge */
        }
    </style>
    </div>



.. raw:: html

    <div class="container mt-5">
    <h2 class="text-center">Manual Card Carousel with Infinite Looping</h2>
    <div id="cardCarousel" class="carousel">
        <div class="carousel-inner" style="display: flex; overflow-x: auto; white-space: nowrap; scrollbar-width: none; -ms-overflow-style: none; transition: none;">
            <!-- Card 1 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <a href="document1.html" class="card-link" style="text-decoration: none; color: inherit; flex: 0 0 auto; margin-right: 15px;">
                        <h5 class="card-title">Card 1</h5>
                        <p class="card-text">Content for Card 1.</p>
                    </a>

                </div>
            </div>
            <!-- Card 2 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <h5 class="card-title">Card 2</h5>
                    <p class="card-text">Content for Card 2.</p>
                </div>
            </div>
            <!-- Card 3 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <h5 class="card-title">Card 3</h5>
                    <p class="card-text">Content for Card 3.</p>
                </div>
            </div>
            <!-- Card 4 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <h5 class="card-title">Card 4</h5>
                    <p class="card-text">Content for Card 4.</p>
                </div>
            </div>
            <!-- Card 5 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <h5 class="card-title">Card 5</h5>
                    <p class="card-text">Content for Card 5.</p>
                </div>
            </div>
            <!-- Card 6 -->
            <div class="card" style="flex: 0 0 auto; width: 250px; margin-right: 15px;">
                <div class="card-body">
                    <h5 class="card-title">Card 6</h5>
                    <p class="card-text">Content for Card 6.</p>
                </div>
            </div>
        </div>
    </div>

    <script>
        const carouselInner = document.querySelector('.carousel-inner');
        const cardWidth = 250 + 15; // Width of each card including margin
        let cardCount = document.querySelectorAll('.carousel-inner .card').length;

        // Function to duplicate the cards to create infinite loop effect
        function cloneCards() {
            const cards = Array.from(document.querySelectorAll('.carousel-inner .card'));
            // Clone the first 3 cards and append to the end
            for (let i = 0; i < 3; i++) {
                carouselInner.appendChild(cards[i].cloneNode(true));
            }
            // Clone the last 3 cards and prepend to the beginning
            for (let i = cardCount - 3; i < cardCount; i++) {
                carouselInner.insertBefore(cards[i].cloneNode(true), carouselInner.firstChild);
            }
        }

        // Wait for the page layout to render, then clone the cards
        window.addEventListener('load', () => {
            // Clone cards to create the infinite loop
            cloneCards();
            
            // Initially set scroll position to the first real card
            carouselInner.scrollLeft = cardWidth * 3;
        });

        // Function to handle infinite scrolling without jumping
        function handleInfiniteScroll() {
            const maxScrollLeft = carouselInner.scrollWidth - carouselInner.clientWidth;
            const currentScrollLeft = carouselInner.scrollLeft;

            // If the user has reached the end (last real card), reset scroll position to first card
            if (currentScrollLeft >= maxScrollLeft - cardWidth) {
                carouselInner.scrollLeft = cardWidth * 3;
            }

            // If the user has reached the start (first real card), reset scroll position to last card
            if (currentScrollLeft <= 0) {
                carouselInner.scrollLeft = cardWidth * (cardCount + 2);
            }
        }

        // Enable smooth scrolling without automatic jumping
        carouselInner.addEventListener('scroll', handleInfiniteScroll);

        // Enable mouse wheel scrolling
        carouselInner.addEventListener('wheel', (event) => {
            if (event.deltaY !== 0) {
                event.preventDefault();
                const scrollSpeed = 2.5; // Adjust multiplier for sensitivity
                carouselInner.scrollLeft += event.deltaY * scrollSpeed;
            }
        });
    </script>

    <style>
        /* Hide the default scrollbar for a cleaner look */
        .carousel-inner {
            scrollbar-width: none; /* For Firefox */
        }

        .carousel-inner::-webkit-scrollbar {
            display: none; /* For Chrome, Safari, and Edge */
        }
    </style>
    </div>





.. raw:: html

   <html>
   <head>
       <style>
           /* Carousel Container */
           .carousel-container {
               position: relative;
               width: 80%;
               margin: 0 auto;
               overflow: hidden;
           }

           /* Carousel Items */
           .carousel-items {
               display: flex;
               transition: transform 0.5s ease-in-out;
           }

           .carousel-item {
               min-width: 100%;
               box-sizing: border-box;
               height: 300px; /* Adjust height as needed */
               background-color: #ddd;
               display: flex;
               justify-content: center;
               align-items: center;
               font-size: 2em;
               color: white;
               border-radius: 10px;
           }

           /* Previous and Next buttons */
           .carousel-button {
               position: absolute;
               top: 50%;
               transform: translateY(-50%);
               background-color: rgba(0, 0, 0, 0.5);
               color: white;
               border: none;
               padding: 10px;
               font-size: 18px;
               cursor: pointer;
           }

           .prev {
               left: 0;
           }

           .next {
               right: 0;
           }
       </style>
   </head>
   <body>
       <div class="carousel-container">
           <div class="carousel-items">
               <div class="carousel-item" style="background-color: #3498db;">Item 1</div>
               <div class="carousel-item" style="background-color: #e74c3c;">Item 2</div>
               <div class="carousel-item" style="background-color: #2ecc71;">Item 3</div>
               <div class="carousel-item" style="background-color: #f39c12;">Item 4</div>
           </div>
           <button class="carousel-button prev" onclick="moveSlide(-1)">&#10094;</button>
           <button class="carousel-button next" onclick="moveSlide(1)">&#10095;</button>
       </div>

       <script>
           let currentIndex = 0;
           const slides = document.querySelectorAll('.carousel-item');
           const totalSlides = slides.length;

           function moveSlide(direction) {
               currentIndex = (currentIndex + direction + totalSlides) % totalSlides;
               document.querySelector('.carousel-items').style.transform = `translateX(-${currentIndex * 100}%)`;
           }

           setInterval(() => moveSlide(1), 3000); // Auto-scroll every 3 seconds
       </script>
   </body>
   </html>


.. raw:: html

   <html>
   <head>
       <style>
           /* Carousel Container */
           .carousel-container {
               position: relative;
               width: 80%;
               margin: 0 auto;
               overflow: hidden;
           }

           /* Carousel Items (Now allowing multiple cards to show) */
           .carousel-items {
               display: flex;
               transition: transform 0.5s ease-in-out;
           }

           .carousel-item {
               min-width: 25%; /* Show 4 cards at a time, adjust as needed */
               box-sizing: border-box;
               height: 300px; /* Adjust height as needed */
               background-color: #ddd;
               display: flex;
               justify-content: center;
               align-items: center;
               font-size: 2em;
               color: white;
               border-radius: 10px;
               margin-right: 10px; /* Space between cards */
           }

           /* Previous and Next buttons */
           .carousel-button {
               position: absolute;
               top: 50%;
               transform: translateY(-50%);
               background-color: rgba(0, 0, 0, 0.5);
               color: white;
               border: none;
               padding: 10px;
               font-size: 18px;
               cursor: pointer;
           }

           .prev {
               left: 0;
           }

           .next {
               right: 0;
           }
       </style>
   </head>
   <body>
       <div class="carousel-container">
           <div class="carousel-items">
               <div class="carousel-item" style="background-color: #3498db;">Item 1</div>
               <div class="carousel-item" style="background-color: #e74c3c;">Item 2</div>
               <div class="carousel-item" style="background-color: #2ecc71;">Item 3</div>
               <div class="carousel-item" style="background-color: #f39c12;">Item 4</div>
               <div class="carousel-item" style="background-color: #9b59b6;">Item 5</div>
               <div class="carousel-item" style="background-color: #1abc9c;">Item 6</div>
               <div class="carousel-item" style="background-color: #16a085;">Item 7</div>
               <div class="carousel-item" style="background-color: #34495e;">Item 8</div>
           </div>
           <button class="carousel-button prev" onclick="moveSlide(-1)">&#10094;</button>
           <button class="carousel-button next" onclick="moveSlide(1)">&#10095;</button>
       </div>

       <script>
           let currentIndex = 0;
           const slides = document.querySelectorAll('.carousel-item');
           const totalSlides = slides.length;
           const visibleCards = 4; // Number of visible cards at once

           function moveSlide(direction) {
               currentIndex = (currentIndex + direction + totalSlides) % totalSlides;
               document.querySelector('.carousel-items').style.transform = `translateX(-${currentIndex * (100 / visibleCards)}%)`;
           }

           setInterval(() => moveSlide(1), 3000); // Auto-scroll every 3 seconds
       </script>
   </body>
   </html>




    