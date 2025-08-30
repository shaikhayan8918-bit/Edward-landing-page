# Edward-landing-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Compact Keywords - The SEO Method for Revenue, Not Just Rankings</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap" rel="stylesheet">
    <style>
        /* CSS Reset */
        *, *::before, *::after {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        html, body {
            overflow-x: hidden;
            width: 100%;
        }

        body {
            background-color: #111827;
            color: #E5E7EB;
            font-family: 'Inter', sans-serif;
            line-height: 1.7;
            -webkit-font-smoothing: antialiased;
        }

        /* --- Layout & Container --- */
        .container {
            width: 100%;
            max-width: 800px;
            margin: 0 auto;
            padding: 0 20px;
        }

        section {
            padding: 80px 0;
            border-bottom: 1px solid #374151;
        }

        section:last-of-type {
            border-bottom: none;
        }

        /* --- Typography --- */
        h1, h2, h3 {
            font-weight: 800;
            line-height: 1.2;
            color: #FFFFFF;
        }

        h1 {
            font-size: 2.5rem;
        }

        h2 {
            font-size: 2rem;
            margin-bottom: 2rem;
            text-align: center;
        }
        
        h2.fascination-headline {
            max-width: 650px;
            margin-left: auto;
            margin-right: auto;
            font-weight: 700;
            font-size: 1.8rem;
            color: #d1d5db;
            border-left: 3px solid #34D399;
            padding-left: 20px;
            text-align: left;
            margin-bottom: 40px;
        }

        p {
            margin-bottom: 1rem;
            font-size: 1.1rem;
            max-width: 700px;
        }

        b, strong {
            font-weight: 700;
            color: #F9FAFB;
        }
        
        .preheader {
            font-size: 0.9rem;
            font-weight: 600;
            color: #34D399;
            text-transform: uppercase;
            letter-spacing: 1px;
            margin-bottom: 1rem;
        }

        .subheader {
            font-size: 1.25rem;
            color: #D1D5DB;
            max-width: 600px;
            margin-top: 1.5rem;
        }
        
        /* --- Hero Section --- */
        .hero {
            text-align: center;
            padding-top: 60px;
            padding-bottom: 60px;
        }
        
        .vsl-icon {
            cursor: pointer;
            width: 100%;
            max-width: 640px;
            margin: 2.5rem auto 2.5rem;
            border-radius: 12px;
            overflow: hidden;
            position: relative;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            border: 1px solid #4B5563;
        }

        .vsl-icon img {
            display: block;
            width: 100%;
            height: auto;
            max-width: 100%;
        }

        .play-button {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 80px;
            height: 80px;
            background-color: rgba(0, 0, 0, 0.6);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: transform 0.2s ease, background-color 0.2s ease;
        }
        .play-button:hover {
            transform: translate(-50%, -50%) scale(1.1);
            background-color: rgba(52, 211, 153, 0.9);
        }
        .play-button svg {
            width: 40px;
            height: 40px;
            fill: #FFFFFF;
            margin-left: 5px;
        }

        /* --- Buttons --- */
        .cta-button {
            display: inline-block;
            background: linear-gradient(to right, #10B981, #34D399);
            color: #064E3B;
            font-size: 1.1rem;
            font-weight: 700;
            text-decoration: none;
            padding: 18px 36px;
            border-radius: 8px;
            box-shadow: 0 4px 15px rgba(52, 211, 153, 0.2);
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 7px 20px rgba(52, 211, 153, 0.3);
            color: #042f23;
        }
        
        .cta-container {
            text-align: center;
            margin-top: 2rem;
        }
        
        /* --- Bullet Points --- */
        .benefit-bullets {
            list-style: none;
            padding: 0;
            margin-top: 2rem;
        }
        .benefit-bullets li {
            display: flex;
            align-items: flex-start;
            font-size: 1.1rem;
            margin-bottom: 1.5rem;
            padding-left: 1.5rem;
            position: relative;
        }
        .benefit-bullets li::before {
            content: '✓';
            color: #34D399;
            font-weight: 800;
            position: absolute;
            left: 0;
            top: 2px;
        }

        /* --- Offer & FAQ Section --- */
        .offer-box, .faq-item {
            background-color: #1F2937;
            border: 1px solid #374151;
            border-radius: 12px;
            padding: 2rem;
            margin-bottom: 2rem;
        }
        
        .price {
            text-align: center;
            margin: 2rem 0;
        }

        .price-main {
            font-size: 3rem;
            font-weight: 800;
            color: #FFFFFF;
        }
        
        .price-note {
            color: #9CA3AF;
            font-size: 0.9rem;
        }
        
        .faq-question {
            font-weight: 700;
            font-size: 1.2rem;
            color: #F9FAFB;
            cursor: pointer;
            position: relative;
            padding-right: 25px;
        }
        .faq-question::after {
            content: '+';
            position: absolute;
            right: 0;
            top: 0;
            font-size: 1.5rem;
            color: #9CA3AF;
            transition: transform 0.2s ease;
        }
        .faq-item.open .faq-question::after {
             transform: rotate(45deg);
        }
        .faq-answer {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out, margin-top 0.3s ease-out;
            color: #D1D5DB;
        }
        .faq-item.open .faq-answer {
             margin-top: 1rem;
        }

        /* --- Responsive Design --- */
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }
            h2, h2.fascination-headline {
                font-size: 1.6rem;
            }
            section {
                padding: 60px 0;
            }
        }
    </style>
</head>
<body>

    <!-- HERO SECTION -->
    <header class="hero">
        <div class="container">
            <p class="preheader">For marketers & founders tired of 'blog & pray' SEO</p>
            <h1>Build High-Converting SEO Landing Pages That Bring In Sales in Weeks...</h1>
            <p class="subheader">...all without writing another 2,000-word blog post that gets zero qualified leads and gets wiped out by the next Google update.</p>
            
            <div class="vsl-icon" role="button" aria-label="Play video about the Compact Keywords method">
                <img src="https://placehold.co/640x360/1f2937/34d399?text=See+How+It+Works" alt="Video thumbnail showing a graph with upward trend">
                <div class="play-button">
                    <svg viewBox="0 0 24 24"><path d="M8 5v14l11-7z"></path></svg>
                </div>
            </div>

            <a href="#offer" class="cta-button">Get The Compact Keywords Method</a>
        </div>
    </header>

    <main>
        <!-- PROBLEM IDENTIFICATION -->
        <section id="problem">
            <div class="container">
                <h2 class="fascination-headline">Does Your SEO Feel Like a Hamster Wheel That Never Stops?</h2>
                <p>You’ve done everything they told you to do.</p>
                <p>You’ve spent months writing long, “definitive” blog posts.</p>
                <p>You’ve chased backlinks, optimized images, and poured money into content that… well… mostly just sits there.</p>
                <p>Maybe a post hits the front page. For a little while. You get a small bump in traffic—vanity metrics that feel good but don’t actually move the needle.</p>
                <p>Then the next Google update hits. And it all disappears overnight.</p>
                <p>Your rankings tank. Your traffic vanishes. And you’re left with a folder full of expensive, useless articles and that sinking feeling in your stomach…</p>
                <p><b>“Am I just invisible to people who are actually ready to buy?”</b></p>
                <p>The cost of doing nothing is more than just wasted time. It’s the sound of your competitors’ phones ringing. It’s another quarter explaining why marketing spend is up but revenue is flat. It's the slow, creeping dread that the game has changed and you've been left behind.</p>
                <p>But what if there's a different way? A leaner, smarter way to get seen by the right people, at the right time.</p>
            </div>
        </section>

        <!-- ORIGIN STORY -->
        <section id="origin">
            <div class="container">
                <h2 class="fascination-headline">How We Broke Free From the "Content Treadmill" by Doing the Opposite of What Gurus Preach</h2>
                <p>For years, the SEO playbook was simple: <b>more is more.</b></p>
                <p>More blog posts. More words. More backlinks. It was a war of attrition. Whoever could produce the most content, the fastest, would eventually win.</p>
                <p>We followed that playbook. We built agencies on it.</p>
                <p>But then something shifted. Google got smarter. AI started summarizing those huge articles we spent weeks writing. Users got tired of scrolling through 3,000 words of fluff to find a simple answer.</p>
                <p>The old model wasn't just inefficient anymore. <b>It was broken.</b></p>
                <p>The breakthrough came when we stopped asking, "How can we rank for this keyword?" and started asking, "What does a person with <i>money in hand</i> actually want when they search this?"</p>
                <p>The answer was almost never a 4,000-word blog post.</p>
                <p>They wanted a clear solution. A direct answer. A page built for conversion, not just information. This led to the discovery of the Compact Keywords method—a system based on precision, not volume.</p>
            </div>
        </section>

        <!-- SOLUTION REVELATION -->
        <section id="solution">
            <div class="container">
                <h2 class="fascination-headline">The 'Compact Keywords' Method: Less Content, More Customers</h2>
                <p>Instead of blogging into the void, this system focuses on building lean, powerful, SEO-optimized <b>landing pages</b> that target people actively looking to make a purchase.</p>
                <p>It’s a system designed for revenue, not just rankings.</p>
                <p>Here’s how it gives you an almost unfair advantage:</p>
                <ul class="benefit-bullets">
                    <li><b>High-Purchase-Intent Keywords ➡</b> We show you how to find the overlooked keywords that signal someone is ready to buy, so you attract qualified leads, not just casual readers. You become a magnet for sales opportunities.</li>
                    <li><b>Lean, SEO-Optimized Landing Pages ➡</b> Get our templates for pages designed to rank quickly and convert, so you can stop wasting time on fluffy blog posts. You become an efficient growth machine.</li>
                    <li><b>A Minimalist Approach to Backlinks ➡</b> Learn how to build authority with fewer, higher-quality links, making you resilient to algorithm updates. You become a trusted authority, not a spammer.</li>
                    <li><b>Future-Proofed for AI ➡</b> This method aligns your site with how AI (like ChatGPT) finds and recommends answers, so you get recommended as the go-to solution. You become part of the answer, not the background noise.</li>
                </ul>
                <p>Imagine seeing multiple conversions within a few months, not years. Imagine outranking bloated competitor blogs with a single, focused landing page.</p>
                <p>This isn't theory. Users of this system are doing it right now.</p>
            </div>
        </section>

        <!-- PRODUCT INTRODUCTION -->
        <section id="product">
            <div class="container">
                 <h2 class="fascination-headline">Inside Compact Keywords: Your Step-by-Step System for Profitable SEO</h2>
                <p>Compact Keywords isn't another library of vague SEO theories. It's a direct, over-the-shoulder action plan.</p>
                <p>You get immediate access to everything you need to start building your SEO sales engine today:</p>
                <div class="offer-box">
                    <ul class="benefit-bullets">
                        <li><b>38 In-Depth Video Modules (~10 hours) ➡</b> Edward walks you through every step of the process, from finding your first keyword to tracking your revenue. No fluff, just actionable steps.</li>
                        <li><b>A Full Suite of Professional Templates ➡</b> Get done-for-you templates for site audits, landing page structure, competitor analysis, and more. This eliminates the guesswork and cuts your implementation time in half.</li>
                        <li><b>15-Week Implementation Guide ➡</b> A clear weekly breakdown that guides you from zero to a fully functioning SEO conversion system, so you're never wondering what to do next.</li>
                        <li><b>On-Page and On-Site SEO Mastery ➡</b> Go beyond keywords and learn the exact site structure that Google loves and that funnels visitors directly toward a sale.</li>
                        <li><b>Advanced Link Building & UGC Tactics ➡</b> See how to get powerful results with a lean approach to links and how to leverage User-Generated Content for explosive growth.</li>
                    </ul>
                </div>
                <p>This system wins because it's built for today's internet. While everyone else is still churning out massive blog posts, you'll be deploying compact, hard-hitting landing pages that attract buyers and drive sales.</p>
            </div>
        </section>
        
        <!-- OFFER STRUCTURE -->
        <section id="offer">
            <div class="container">
                <h2 class="fascination-headline">Get Lifetime Access to the Complete Compact Keywords System</h2>
                <p>You're at a crossroads. You can continue on the content treadmill, hoping the next blog post is the one that finally works...</p>
                <p>Or you can get a proven system to turn your SEO efforts into a predictable source of revenue.</p>
                <p>When you join today, you get complete, lifetime access to everything:</p>
                <ul class="benefit-bullets">
                    <li>All 38+ video modules</li>
                    <li>The complete template library</li>
                    <li>The 15-week implementation plan</li>
                    <li>All future updates to the course</li>
                </ul>
                <div class="price">
                    <div class="price-main">$499</div>
                    <div class="price-note">One-time payment. Lifetime access.</div>
                </div>
                
                <div class="cta-container">
                    <a href="#purchase-link" class="cta-button">Buy Compact Keywords Now</a>
                </div>
                <p style="text-align:center; font-size: 0.9rem; margin-top: 1rem; color: #9CA3AF;">Some users report earning back their investment multiple times over within months.</p>
                <p style="margin-top: 2rem;"><b>A word of warning:</b> Google's next core update is always around the corner. The "blog and pray" model is getting riskier by the day. This is your chance to build a resilient SEO strategy that doesn't just survive updates, but gets stronger because of them. The time to act is now, before you're forced to.</p>

            </div>
        </section>

        <!-- FAQ SECTION -->
        <section id="faq">
            <div class="container">
                <h2 class="fascination-headline">What's Holding You Back?</h2>
                
                <div class="faq-item">
                    <div class="faq-question">"Is this really worth $499?"</div>
                    <div class="faq-answer">
                        <p>Think about the cost of what you're doing now. The hours spent on content that doesn't convert. The money spent on writers. The sales you're missing every single month. Users have reported a 6x return on their investment. This isn't an expense; it's a direct investment in a system built for ROI.</p>
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">"I'm not an SEO expert. Is this too advanced for me?"</div>
                    <div class="faq-answer">
                        <p>Quite the opposite. This course was designed to give you a clear, step-by-step path, even if you're starting with limited SEO knowledge. The templates and bite-sized video modules are made to be implemented, not just studied. If you can follow a recipe, you can follow this system.</p>
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">"How is this different from all the other SEO courses out there?"</div>
                    <div class="faq-answer">
                        <p>Most SEO courses are still teaching the old, broken model of "more content, more blogs." Compact Keywords is the only system focused exclusively on building lean, high-converting landing pages that target bottom-of-funnel, purchase-intent keywords. It's about sales, not just traffic.</p>
                    </div>
                </div>

                <div class="faq-item">
                    <div class="faq-question">"How much time will this take to implement?"</div>
                    <div class="faq-answer">
                        <p>The course itself is about 10 hours of video. But the real value is in the time it *saves* you. With the templates and clear action plan, you'll be spending your time on high-impact tasks that generate revenue, not on writing endless blog posts. You can work through it at your own pace, but the system is designed for efficiency.</p>
                    </div>
                </div>
                
                <div class="cta-container" style="margin-top: 3rem;">
                     <a href="#purchase-link" class="cta-button">Start Building Your SEO Sales Engine</a>
                </div>
            </div>
        </section>
    </main>

    <script>
        document.addEventListener('DOMContentLoaded', function () {
            const faqItems = document.querySelectorAll('.faq-item');

            faqItems.forEach(item => {
                const question = item.querySelector('.faq-question');
                const answer = item.querySelector('.faq-answer');

                question.addEventListener('click', () => {
                    const isOpen = item.classList.contains('open');

                    // Close all items
                    faqItems.forEach(i => {
                        i.classList.remove('open');
                        i.querySelector('.faq-answer').style.maxHeight = '0px';
                         i.querySelector('.faq-answer').style.marginTop = '0px';
                    });

                    // If the clicked item was closed, open it
                    if (!isOpen) {
                        item.classList.add('open');
                        answer.style.maxHeight = answer.scrollHeight + "px";
                        answer.style.marginTop = '1rem';
                    }
                });
            });
        });
    </script>

</body>
</html>

