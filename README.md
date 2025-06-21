<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Rabenda Spa - Japońskie Rytuały Wellness</title>
      <link rel="stylesheet" href="style.css" />
    <link href="https://fonts.googleapis.com/css2?family=Julius+Sans+One:wght@400&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet" />
</head>
<body>
    <div class="container">
        <!-- Header -->
        <header class="header">
            <nav class="nav-menu">
                <a href="#about" class="nav-link">O nas</a>
                <a href="#services" class="nav-link">Zabiegi</a>
                <a href="#pricing" class="nav-link">Cennik</a>
                <a href="#gallery" class="nav-link">Galeria</a>
                <a href="#contact" class="nav-link">Kontakt</a>
            </nav>
            <img src="logo.jpg" alt="Rabenda Spa Logo" class="logo" />
        </header>

        <!-- Hero Section -->
        <section id="about" class="hero-section">
            <div class="hero-image"></div>
            <div class="hero-content">
                <h1 class="hero-title">O nas</h1>
                <p class="hero-text">  Wierzymy, że piękno i harmonia rodzą się z troski o ciało, umysł 
i duszę. Nasze miejsce powstało z pasji do natury, aromaterapii 
i głębokiego relaksu. Otuleni zapachem lawendy, zapraszamy Cię do świata spokoju, gdzie każdy detal został stworzony 
z myślą o Twoim komforcie.</p>
            </div>
        </section>

        <!-- Gallery Section -->
        <section id="gallery" class="gallery-section">
            <h2 class="section-title">Galeria</h2>
            <div class="gallery-container">
                <button class="gallery-nav-btn" onclick="previousSlide()">
                    <img src="2.png" alt="Previous" style="width: 29px; height: 56px;" />
                </button>
                <div class="gallery-slider">
                    <div class="gallery-item"></div>
                    <div class="gallery-item"></div>
                    <div class="gallery-item"></div>
                </div>
                <button class="gallery-nav-btn" onclick="nextSlide()">
                    <img src="1.png" alt="Next" style="width: 29px; height: 56px;" />
                </button>
            </div>
        </section>

        <!-- Services Section -->
        <section id="services" class="services-section">
            <h2 class="section-title">Zabiegi</h2>
            <div class="services-grid">
                <!-- Service 1: Rytuał Onsen -->
                <div class="service-card">
                    <div class="service-content">
                        <div class="service-image-container">
                            <div class="service-image"></div>
                            <h3 class="service-title">Rytuał Onsen</h3>
                        </div>
                        <p class="service-description">Aromatyczna kąpiel w lawendowej soli mineralnej, połączona 
z delikatnym masażem głowy 
i karku. Idealny na stres 
i napięcia dnia codziennego.</p>
                        <button class="service-btn" onclick="bookService('Rytuał Onsen')">Rezerwuj</button>
                    </div>
                </div>

                <!-- Service 2: Shiatsu -->
                <div class="service-card">
                    <div class="service-content">
                        <div class="service-image-container">
                            <div class="service-image"></div>
                            <h3 class="service-title">Shiatsu</h3>
                        </div>
                        <p class="service-description">Japoński masaż uciskowy na bazie punktów meridianowych, wykonywany z użyciem naturalnego olejku lawendowego. Przywraca równowagę energetyczną i głęboko odpręża.</p>
                        <button class="service-btn" onclick="bookService('Shiatsu')">Rezerwuj</button>
                    </div>
                </div>

                <!-- Service 3: Rytuał Kobido -->
                <div class="service-card">
                    <div class="service-content">
                        <div class="service-image-container">
                            <div class="service-image"></div>
                            <h3 class="service-title">Rytuał Kobido</h3>
                        </div>
                        <p class="service-description">Ekskluzywny japoński liftingujący masaż twarzy Kobido połączony 
z aromaterapią i maseczką lawendową.
<strong>Efekt: rozświetlona cera 
i wyciszony umysł.</strong></p>
                        <button class="service-btn" onclick="bookService('Rytuał Kobido')">Rezerwuj</button>
                    </div>
                </div>

                <!-- Service 4: Yin & Yang -->
                <div class="service-card">
                    <div class="service-content">
                        <div class="service-image-container">
                            <div class="service-image"></div>
                            <h3 class="service-title">Yin & Yang</h3>
                        </div>
                        <p class="service-description">Zabieg rozpoczyna się peelingiem z kwiatów lawendy i ryżu, następnie aplikowany jest nawilżający balsam z dodatkiem japońskiej kamelii. Balans dla ciała i ducha.</p>
                        <button class="service-btn" onclick="bookService('Yin & Yang')">Rezerwuj</button>
                    </div>
                </div>

                <!-- Service 5: Zen Lavendari -->
                <div class="service-card">
                    <div class="service-content">
                        <div class="service-image-container">
                            <div class="service-image"></div>
                            <h3 class="service-title">Zen Lavendari</h3>
                        </div>
                        <p class="service-description">Relaksacyjny rytuał dla stóp: kąpiel w ciepłej wodzie z lawendą, masaż stóp i refleksologia według japońskiej tradycji.
 Idealny wstęp do innych zabiegów.</p>
                        <button class="service-btn" onclick="bookService('Zen Lavendari')">Rezerwuj</button>
                    </div>
                </div>

                <!-- Service 6: Sen Lawendy -->
                <div class="service-card">
                    <div class="service-content">
                        <div class="service-image-container">
                            <div class="service-image"></div>
                            <h3 class="service-title">Sen Lawendy</h3>
                        </div>
                        <p class="service-description">Wieczorny masaż całego ciała z ciepłym olejem lawendowym 
i technikami japońskiej aromaterapii. Pomaga głęboko się wyciszyć i przygotować do snu.</p>
                        <button class="service-btn" onclick="bookService('Sen Lawendy')">Rezerwuj</button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Reviews Section -->
        <section class="reviews-section">
            <h2 class="section-title">Opinie</h2>
            <div class="reviews-container">
                <div class="review-card">
                    <div class="review-header">
                        <div class="review-avatar"></div>
                        <span class="review-name">Anna, 34 lata</span>
                        <div class="review-stars">
                            <div class="star"></div>
                            <div class="star"></div>
                            <div class="star"></div>
                            <div class="star"></div>
                            <div class="star"></div>
                        </div>
                    </div>
                    <p class="review-text">"To było dokładnie to, czego potrzebowałam! Cisza, zapach lawendy i profesjonalne podejście sprawiły, że pierwszy raz od dawna naprawdę się zrelaksowałam. Masaż Kobido był niesamowity – czuję się młodziej!"</p>
                </div>

                <div class="review-card">
                    <div class="review-header">
                        <div class="review-avatar"></div>
                        <span class="review-name">Natalia, 30 lat</span>
                        <div class="review-stars">
                            <div class="star"></div>
                            <div class="star"></div>
                            <div class="star"></div>
                            <div class="star"></div>
                            <div class="star"></div>
                        </div>
                    </div>
                    <p class="review-text">"Byłam w wielu spa, ale tu jest coś wyjątkowego. Japońskie rytuały w połączeniu z lawendą to strzał w dziesiątkę. Relaks na najwyższym poziomie. Polecam z całego serca!"</p>
                </div>

                <button class="reviews-nav" onclick="nextReview()">
                    <img src="1.png" alt="Next Review" style="width: 29px; height: 56px;" />
                </button>
            </div>
        </section>

        <!-- Booking Section -->
        <section class="booking-section">
            <h2 class="section-title">Rezerwacja</h2>
            <p class="booking-subtitle">Zasługujesz na chwilę tylko dla siebie. Umów się już dziś.</p>
            
            <form class="booking-form" onsubmit="submitBooking(event)">
                <div class="form-group">
                    <label class="form-label">Imie i nazwisko</label>
                    <input type="text" class="form-input" name="fullName" required />
                </div>

                <div class="form-group">
                    <label class="form-label">e-mail</label>
                    <input type="email" class="form-input" name="email" required />
                </div>

                <div class="form-group">
                    <label class="form-label">numer telefonu</label>
                    <input type="tel" class="form-input" name="phone" required />
                </div>

                <div class="form-group">
                    <label class="form-label">zabieg</label>
                    <div class="form-dropdown" onclick="toggleDropdown('service')">
                        <span id="selectedService">Wybierz zabieg</span>
                        <div class="dropdown-arrow">
                            <img src="dol.png" alt="Dropdown" style="width: 42px; height: 29px;" />
                        </div>
                    </div>
                    <select name="service" id="serviceSelect" style="display: none;">
                        <option value>Wybierz zabieg</option>
                        <option value="Rytuał Onsen">Rytuał Onsen</option>
                        <option value="Shiatsu">Shiatsu</option>
                        <option value="Rytuał Kobido">Rytuał Kobido</option>
                        <option value="Yin & Yang">Yin & Yang</option>
                        <option value="Zen Lavendari">Zen Lavendari</option>
                        <option value="Sen Lawendy">Sen Lawendy</option>
                    </select>
                </div>

                <div class="form-group">
                    <label class="form-label">data i godzina</label>
                    <div class="form-dropdown" onclick="toggleDropdown('datetime')">
                        <span id="selectedDateTime">Wybierz datę i godzinę</span>
                        <div class="dropdown-arrow">
                            <img src="dol.png" alt="Dropdown" style="width: 42px; height: 29px;" />
                        </div>
                    </div>
                    <input type="datetime-local" name="datetime" id="datetimeInput" style="display: none;" />
                </div>

                <div class="form-group">
                    <label class="form-label">uwagi</label>
                    <div style="position: relative;">
                        <textarea class="form-textarea" name="comments" maxlength="300" oninput="updateCounter(this)"></textarea>
                        <div class="textarea-counter">0/300 słów</div>
                    </div>
                </div>

                <div class="checkbox-group">
                    <input type="checkbox" class="checkbox" name="consent" required />
                    <label class="checkbox-label">Wyrażam zgodę na przetwarzanie moich danych osobowych w celu realizacji rezerwacji zgodnie z polityką prywatności.</label>
                </div>

                <button type="submit" class="submit-btn">ZAREZERWUJ</button>
            </form>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="contact-section">
            <h2 class="section-title">Kontakt</h2>
            <p class="contact-subtitle">Miejsce, gdzie harmonia ciała i ducha spotyka się z aromatem lawendy.</p>
            
            <div class="contact-content">
                <div class="contact-info">
                    <div class="contact-hours">
                        <strong>Godziny otwarcia:</strong> Pon – Pt: 10:00 – 20:00 Sobota: 10:00 – 18:00 Niedziela: zamknięte
                    </div>
                    <div class="contact-social">
                        <strong>Social Media:</strong>
<strong>Instagram:</strong> @rabenda_spa
<strong>Facebook:</strong> Rabenda Spa
<strong>TikTok:</strong> @rabenda_spa
                    </div>
                </div>
                <div>
                    <div class="contact-map"></div>
                    <div class="contact-address">ul. Kwiatowa 12, 00-123 Warszawa
tel. +48 123 456 789
kontakt@rabendaspa.pl</div>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer class="footer">
            <p class="footer-text">© 2025 Rabenda Spa. Wszystkie prawa zastrzeżone.</p>
            <img src="logo.jpg" alt="Rabenda Spa Logo" class="footer-logo" />
        </footer>
    </div>

    <script>
        // Gallery slider functionality
        let currentSlide = 0;
        const totalSlides = 3;

        function nextSlide() {
            currentSlide = (currentSlide + 1) % totalSlides;
            updateGallery();
        }

        function previousSlide() {
            currentSlide = (currentSlide - 1 + totalSlides) % totalSlides;
            updateGallery();
        }

        function updateGallery() {
            // Add animation or update gallery display
            console.log('Current slide:', currentSlide);
        }

        // Reviews navigation
        let currentReview = 0;
        const reviews = document.querySelectorAll('.review-card');

        function nextReview() {
            reviews[currentReview].style.display = 'none';
            currentReview = (currentReview + 1) % reviews.length;
            reviews[currentReview].style.display = 'block';
        }

        // Service booking
        function bookService(serviceName) {
            document.getElementById('selectedService').textContent = serviceName;
            document.getElementById('serviceSelect').value = serviceName;
            document.querySelector('[href="#booking"]')?.scrollIntoView({ behavior: 'smooth' });
        }

        // Dropdown functionality
        function toggleDropdown(type) {
            if (type === 'service') {
                const options = [
                    'Rytuał Onsen',
                    'Shiatsu', 
                    'Rytuał Kobido',
                    'Yin & Yang',
                    'Zen Lavendari',
                    'Sen Lawendy'
                ];
                
                const selectedOption = prompt('Wybierz zabieg:\
' + options.map((opt, i) => `${i+1}. ${opt}`).join('\
'));
                if (selectedOption && selectedOption >= 1 && selectedOption <= options.length) {
                    const service = options[selectedOption - 1];
                    document.getElementById('selectedService').textContent = service;
                    document.getElementById('serviceSelect').value = service;
                }
            } else if (type === 'datetime') {
                const datetime = prompt('Wprowadź datę i godzinę (YYYY-MM-DD HH:MM):');
                if (datetime) {
                    document.getElementById('selectedDateTime').textContent = datetime;
                    document.getElementById('datetimeInput').value = datetime;
                }
            }
        }

        // Textarea counter
        function updateCounter(textarea) {
            const counter = textarea.parentNode.querySelector('.textarea-counter');
            const wordCount = textarea.value.split(/\s+/).filter(word => word.length > 0).length;
            counter.textContent = `${wordCount}/300 słów`;
        }

        // Form submission
        function submitBooking(event) {
            event.preventDefault();
            
            const formData = new FormData(event.target);
            const bookingData = {
                fullName: formData.get('fullName'),
                email: formData.get('email'),
                phone: formData.get('phone'),
                service: formData.get('service') || document.getElementById('selectedService').textContent,
                datetime: formData.get('datetime') || document.getElementById('selectedDateTime').textContent,
                comments: formData.get('comments'),
                consent: formData.get('consent')
            };

            // Simulate booking submission
            alert('Dziękujemy za rezerwację! Skontaktujemy się z Państwem w ciągu 24 godzin.');
            console.log('Booking data:', bookingData);
            
            // Reset form
            event.target.reset();
            document.getElementById('selectedService').textContent = 'Wybierz zabieg';
            document.getElementById('selectedDateTime').textContent = 'Wybierz datę i godzinę';
        }

        // Smooth scrolling for navigation
        document.querySelectorAll('.nav-link').forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                const targetSection = document.querySelector(targetId);
                if (targetSection) {
                    targetSection.scrollIntoView({ behavior: 'smooth' });
                }
            });
        });

        // Initialize reviews display
        document.addEventListener('DOMContentLoaded', function() {
            reviews.forEach((review, index) => {
                if (index !== 0) {
                    review.style.display = 'none';
                }
            });
        });

        // Checkbox styling
        document.querySelectorAll('.checkbox').forEach(checkbox => {
            checkbox.addEventListener('change', function() {
                if (this.checked) {
                    this.style.backgroundColor = '#a777e5';
                } else {
                    this.style.backgroundColor = '#ffffff';
                }
            });
        });

        // Form validation
        document.querySelectorAll('.form-input').forEach(input => {
            input.addEventListener('blur', function() {
                if (this.value.trim() === '') {
                    this.style.borderColor = '#ff6b6b';
                } else {
                    this.style.borderColor = '#a777e5';
                }
            });
        });

        // Hover effects for buttons
        document.querySelectorAll('.service-btn, .submit-btn, .gallery-nav-btn').forEach(btn => {
            btn.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-2px)';
                this.style.boxShadow = '0 4px 12px rgba(167, 119, 229, 0.3)';
            });
            
            btn.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0)';
                this.style.boxShadow = 'none';
            });
        });
    </script>
</body>
</html>
