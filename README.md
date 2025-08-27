# Thanu
Web development practice repo – HTML, CSS, JavaScript examples and projects
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Thanu - The Beauty of Small Moments</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Georgia', serif;
            line-height: 1.8;
            color: #2c3e50;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        .card {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 60px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            margin-bottom: 30px;
        }

        .header {
            text-align: center;
            margin-bottom: 50px;
        }

        .logo {
            font-size: 2.8em;
            font-weight: bold;
            background: linear-gradient(135deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 10px;
        }

        .subtitle {
            font-size: 1.1em;
            color: #7f8c8d;
            font-style: italic;
        }

        h1 {
            font-size: 2.8em;
            margin-bottom: 40px;
            text-align: center;
            color: #2c3e50;
            font-weight: 300;
        }

        h2 {
            font-size: 1.6em;
            margin: 40px 0 20px 0;
            color: #34495e;
            font-weight: 400;
            border-bottom: 2px solid rgba(102, 126, 234, 0.2);
            padding-bottom: 10px;
        }

        p {
            font-size: 1.1em;
            margin-bottom: 25px;
            text-align: justify;
            color: #34495e;
        }

        .highlight {
            background: linear-gradient(120deg, rgba(102, 126, 234, 0.15) 0%, rgba(118, 75, 162, 0.15) 100%);
            padding: 2px 6px;
            border-radius: 4px;
            font-weight: 500;
        }

        .floating-elements {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .floating-element {
            position: absolute;
            opacity: 0.12;
            animation: float 25s infinite linear;
            font-size: 1.5em;
        }

        @keyframes float {
            0% { transform: translateY(100vh) rotate(0deg); }
            100% { transform: translateY(-100px) rotate(360deg); }
        }

        .floating-element:nth-child(1) { left: 5%; animation-delay: 0s; }
        .floating-element:nth-child(2) { left: 15%; animation-delay: -3s; }
        .floating-element:nth-child(3) { left: 25%; animation-delay: -6s; }
        .floating-element:nth-child(4) { left: 35%; animation-delay: -9s; }
        .floating-element:nth-child(5) { left: 45%; animation-delay: -12s; }
        .floating-element:nth-child(6) { left: 55%; animation-delay: -15s; }
        .floating-element:nth-child(7) { left: 65%; animation-delay: -18s; }
        .floating-element:nth-child(8) { left: 75%; animation-delay: -21s; }
        .floating-element:nth-child(9) { left: 85%; animation-delay: -24s; }
        .floating-element:nth-child(10) { left: 95%; animation-delay: -27s; }

        .content {
            position: relative;
            z-index: 10;
        }

        .section {
            margin-bottom: 40px;
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.8s ease, transform 0.8s ease;
        }

        .section.visible {
            opacity: 1;
            transform: translateY(0);
        }

        .quote-style {
            font-style: italic;
            color: #5a6c7d;
            border-left: 4px solid #667eea;
            padding-left: 20px;
            margin: 30px 0;
        }

        @media (max-width: 768px) {
            .container {
                padding: 20px 15px;
            }
            
            .card {
                padding: 30px;
                border-radius: 15px;
            }
            
            h1 {
                font-size: 2.2em;
            }

            h2 {
                font-size: 1.4em;
            }
            
            .logo {
                font-size: 2.2em;
            }
            
            p {
                font-size: 1em;
                text-align: left;
            }

            .floating-element {
                font-size: 1.2em;
            }
        }
    </style>
</head>
<body>
    <div class="floating-elements">
        <div class="floating-element">☀️</div>
        <div class="floating-element">🌸</div>
        <div class="floating-element">☕</div>
        <div class="floating-element">🌙</div>
        <div class="floating-element">🍃</div>
        <div class="floating-element">✨</div>
        <div class="floating-element">🌅</div>
        <div class="floating-element">💫</div>
        <div class="floating-element">🌺</div>
        <div class="floating-element">🦋</div>
    </div>

    <div class="container content">
        <div class="card">
            <div class="header">
                <div class="logo">Thanu</div>
                <div class="subtitle">Discovering beauty in life's gentle moments</div>
            </div>

            <h1>The Beauty of Small Moments</h1>

            <div class="section">
                <p>In a world that constantly celebrates the extraordinary, the monumental, and the grand, we often overlook the profound beauty that exists in the smallest corners of our daily existence. Sometimes, the most beautiful parts of life are not the grand achievements or picture-perfect milestones we set out to capture, but the little, fleeting moments that often slip quietly by like whispers in the wind.</p>
            </div>

            <div class="section">
                <h2>The Poetry of Morning Light</h2>
                <p>Consider the <span class="highlight">warmth of morning sunlight</span> streaming gently through your window, painting golden patterns across the floor in an ever-shifting dance of light and shadow. This simple phenomenon, repeated countless times throughout our lives, carries within it a quiet majesty that rivals any masterpiece hanging in the world's greatest galleries. The way dust motes float lazily through these beams of light, creating their own miniature galaxies, speaks to something profound about presence and peace.</p>
                
                <p>There's something almost sacred about those first moments of awakening when the world is still soft around the edges, before the day has fully taken shape. The gentle transition from sleep to consciousness, the gradual awareness of warmth and light, the slow unfurling of another day's possibilities—these are not merely biological processes but profound experiences of renewal and hope.</p>
            </div>

            <div class="section">
                <h2>The Resonance of Human Connection</h2>
                <p>It's the <span class="highlight">soft laughter</span> you share with a friend that lingers long after the conversation ends, echoing in your heart like the last notes of a beautiful song. These moments of genuine connection transcend the words spoken; they create invisible threads that bind us to one another across time and distance. The spontaneous burst of joy, the understanding glance, the comfortable silence shared between kindred spirits—these interactions remind us that we are not alone in our journey through life.</p>
                
                <p>Think of the last time someone truly listened to you, not just waiting for their turn to speak, but genuinely absorbing your words with their whole being. Remember how that felt—the validation, the sense of being seen and understood. These moments of authentic human connection are perhaps the most precious gifts we can give and receive, yet they cost nothing and require only our presence.</p>
            </div>

            <div class="section">
                <h2>The Ritual of Daily Comfort</h2>
                <p>It's the comforting ritual of <span class="highlight">sipping a cup of tea</span> after a long, tiring day—a pause, a breath, a reminder that you are here, alive, and allowed to simply be. This simple act becomes a bridge between the chaos of the day and the peace of evening. The warmth of the cup in your hands, the aromatic steam rising like incense, the first sip that seems to wash away the accumulated stress of hours—these elements combine to create a moment of pure mindfulness.</p>
                
                <p>Such rituals anchor us in the present moment and provide structure to our days. Whether it's the morning coffee that signals the start of a new day, the evening walk that helps transition from work to rest, or the bedtime routine that prepares us for sleep, these small ceremonies create rhythm and meaning in our lives. They are the punctuation marks in the run-on sentence of our busy existence.</p>
            </div>

            <div class="section">
                <h2>The Quiet Magic of the Ordinary</h2>
                <p>These small moments are not loud or demanding. They don't need applause or recognition. They don't require stage lights or red carpets. Yet, they carry a <span class="highlight">quiet magic</span> that can soothe the heart and ground the soul in ways that grand spectacles often cannot. They work their influence subtly, like gentle rain nurturing seeds we didn't even know we had planted in our hearts.</p>
                
                <p>The magic lies not in their drama but in their consistency, not in their rarity but in their availability. They are democratically distributed across all lives, regardless of circumstance or status. A person living in a mansion and someone in a modest apartment can both witness the same sunset, feel the same cool breeze, experience the same moment of unexpected joy when a favorite song plays on the radio.</p>
            </div>

            <div class="section">
                <h2>Finding Beauty in the Everyday</h2>
                <p>They remind us that beauty does not always need to be discovered in extraordinary places—often, it is already nestled within the rhythm of our everyday lives, waiting patiently to be noticed and appreciated. The way shadows shift across a wall as the day progresses, the sound of children playing in a distant park, the feeling of cool sheets against skin at the end of a warm day—these are the building blocks of a beautiful life.</p>
                
                <p>This doesn't mean that extraordinary experiences aren't valuable or meaningful. Travel, achievements, celebrations, and milestones certainly have their place in a rich and full life. But when we place all our hope for happiness and fulfillment on these peak experiences, we risk missing the vast landscape of joy that surrounds us every single day.</p>
            </div>

            <div class="section">
                <h2>The Art of Awareness</h2>
                <p>When we learn to notice these gentle threads of joy woven into ordinary days, life feels different. The weight of routine seems lighter, the world looks brighter, and meaning reveals itself in the simplest forms. It's like adjusting the focus on a camera—suddenly, details that were always there become clear and sharp, revealing beauty that was hiding in plain sight.</p>
                
                <p>This shift in awareness doesn't happen overnight. It requires practice, patience, and a willingness to slow down in a world that seems determined to speed up. It means choosing <span class="highlight">presence over productivity</span>, at least in small doses. It means training ourselves to notice the texture of experiences, not just their outcomes.</p>
            </div>

            <div class="section">
                <h2>Small Treasures, Infinite Worth</h2>
                <p>A <span class="highlight">handwritten note</span> tucked into a lunch bag, the <span class="highlight">scent of the earth after rain</span> that carries whispers of renewal and growth, the <span class="highlight">comfortable silence</span> shared in the company of someone you love—these are treasures that require nothing but awareness to feel complete. They don't need to be earned or purchased or achieved. They simply need to be received with an open heart and a receptive spirit.</p>
                
                <p>The handwritten note speaks of thoughtfulness and care in an age of digital communication. The petrichor after rain connects us to the ancient cycles of earth and sky. The comfortable silence with a loved one represents a kind of intimacy that goes beyond words—the profound peace of being fully accepted just as we are.</p>
            </div>

            <div class="section">
                <h2>The Practice of Presence</h2>
                <p>Perhaps the greatest gift we can give ourselves is not rushing past these moments in search of something greater, but <span class="highlight">embracing them fully</span>, allowing them to fill us with their quiet wisdom and gentle grace. This requires a fundamental shift in how we define success and fulfillment. Instead of always reaching for the next thing, the bigger thing, the better thing, we can learn to sink into the richness of what is already here.</p>
                
                <p>This practice of presence is both simple and challenging. Simple because it requires no special equipment, no training, no expertise—just the willingness to pay attention. Challenging because our minds are often elsewhere, planning the future or replaying the past, missing the only moment we actually have: this one.</p>
            </div>

            <div class="section">
                <h2>Building a Life of Moments</h2>
                <p class="quote-style">For when we do embrace these small moments fully, we realize that life is not built solely upon milestones or achievements, but upon countless small moments—each one carrying a quiet beauty that, together, creates a life worth cherishing.</p>
                
                <p>Like individual brushstrokes that combine to create a masterpiece, or single notes that weave together to form a symphony, these moments accumulate into something magnificent. The morning coffee, the evening sunset, the text from a friend, the comfortable shoes, the favorite song on the radio, the unexpected compliment, the perfect temperature day—each small treasure contributing to the greater whole of a life lived with awareness and appreciation.</p>
            </div>
        </div>
    </div>

    <script>
        // Intersection Observer for fade-in animations
        const observer = new IntersectionObserver((entries) => {
            entries.forEach((entry) => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        });

        // Observe all sections
        document.querySelectorAll('.section').forEach((section) => {
            observer.observe(section);
        });

        // Parallax effect for floating elements
        window.addEventListener('scroll', () => {
            const scrolled = window.pageYOffset;
            const parallax = document.querySelector('.floating-elements');
            const speed = scrolled * 0.3;
            parallax.style.transform = `translateY(${speed}px)`;
        });

        // Add smooth scroll behavior
        document.documentElement.style.scrollBehavior = 'smooth';
    </script>
</body>
</html>
