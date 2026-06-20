# SMT [smt.form.html](https://github.com/user-attachments/files/29155908/smt.form.html)
<artifact identifier="smt-recruitment-v2" type="text/html" title="SMT Recruitment Form - Gold/Black Edition"> <!DOCTYPE html> <html lang="en"> <head> <meta charset="UTF-8"> <meta name="viewport" content="width=device-width, initial-scale=1.0"> <title>SMT Recruitment - Slither Master's Team</title> <style> * { margin: 0; padding: 0; box-sizing: border-box; }
body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background: linear-gradient(135deg, #0a0a0a 0%, #1a1a1a 50%, #0f0f0f 100%);
        color: #e0e0e0;
        min-height: 100vh;
        padding: 20px;
        position: relative;
        overflow-x: hidden;
    }

    body::before {
        content: '';
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        bottom: 0;
        background-image: 
            repeating-linear-gradient(45deg, transparent, transparent 10px, rgba(201, 168, 76, 0.03) 10px, rgba(201, 168, 76, 0.03) 20px),
            repeating-linear-gradient(-45deg, transparent, transparent 10px, rgba(201, 168, 76, 0.03) 10px, rgba(201, 168, 76, 0.03) 20px);
        pointer-events: none;
        z-index: 1;
    }

    .container {
        max-width: 800px;
        margin: 0 auto;
        position: relative;
        z-index: 2;
    }

    .hero {
        text-align: center;
        padding: 60px 20px;
        background: linear-gradient(135deg, rgba(201, 168, 76, 0.1) 0%, rgba(0, 0, 0, 0.4) 100%);
        border-radius: 20px;
        margin-bottom: 40px;
        border: 2px solid rgba(201, 168, 76, 0.3);
        box-shadow: 0 20px 60px rgba(201, 168, 76, 0.2);
        backdrop-filter: blur(10px);
    }

    .logo-foundation {
        position: relative;
        display: inline-block;
        margin-bottom: 20px;
    }

    .team-name {
        font-size: 72px;
        font-weight: 900;
        background: linear-gradient(135deg, #C9A84C 0%, #FFD700 50%, #C9A84C 100%);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
        letter-spacing: 8px;
        text-shadow: 0 0 30px rgba(201, 168, 76, 0.5);
        filter: drop-shadow(0 4px 12px rgba(201, 168, 76, 0.4));
    }

    .tagline {
        font-size: 20px;
        color: #C9A84C;
        letter-spacing: 4px;
        margin-bottom: 10px;
        font-weight: 600;
    }

    .subtitle {
        font-size: 16px;
        color: #999;
        font-style: italic;
    }

    .stats-grid {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 20px;
        margin: 30px 0;
    }

    .stat-card {
        background: rgba(20, 20, 20, 0.8);
        padding: 25px;
        border-radius: 12px;
        border: 1px solid rgba(201, 168, 76, 0.3);
        text-align: center;
        transition: all 0.3s ease;
    }

    .stat-card:hover {
        transform: translateY(-5px);
        border-color: #C9A84C;
        box-shadow: 0 10px 30px rgba(201, 168, 76, 0.3);
    }

    .stat-number {
        font-size: 32px;
        font-weight: bold;
        color: #C9A84C;
        margin-bottom: 8px;
    }

    .stat-label {
        font-size: 13px;
        color: #888;
        text-transform: uppercase;
        letter-spacing: 1px;
    }

    .section {
        background: rgba(20, 20, 20, 0.6);
        backdrop-filter: blur(10px);
        border-radius: 16px;
        padding: 40px;
        margin-bottom: 30px;
        border: 1px solid rgba(201, 168, 76, 0.2);
        box-shadow: 0 8px 32px rgba(0, 0, 0, 0.4);
    }

    .section-header {
        display: flex;
        align-items: center;
        margin-bottom: 30px;
        padding-bottom: 15px;
        border-bottom: 2px solid rgba(201, 168, 76, 0.3);
    }

    .section-number {
        width: 40px;
        height: 40px;
        background: linear-gradient(135deg, #C9A84C, #8B7355);
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        font-weight: bold;
        font-size: 18px;
        margin-right: 15px;
        color: #000;
    }

    .section-title {
        font-size: 24px;
        font-weight: 600;
        color: #C9A84C;
    }

    .form-group {
        margin-bottom: 25px;
    }

    label {
        display: block;
        margin-bottom: 8px;
        color: #C9A84C;
        font-weight: 500;
        font-size: 14px;
    }

    .required {
        color: #ff6b6b;
        margin-left: 4px;
    }

    input[type="text"],
    input[type="number"],
    input[type="url"],
    textarea,
    select {
        width: 100%;
        padding: 12px 16px;
        background: rgba(30, 30, 30, 0.8);
        border: 1px solid rgba(201, 168, 76, 0.3);
        border-radius: 8px;
        color: #e0e0e0;
        font-size: 15px;
        transition: all 0.3s ease;
    }

    input:focus,
    textarea:focus,
    select:focus {
        outline: none;
        border-color: #C9A84C;
        box-shadow: 0 0 0 3px rgba(201, 168, 76, 0.2);
    }

    textarea {
        resize: vertical;
        min-height: 100px;
        font-family: inherit;
    }

    .region-grid {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 15px;
    }

    .region-card {
        background: rgba(30, 30, 30, 0.6);
        border: 2px solid rgba(201, 168, 76, 0.2);
        border-radius: 12px;
        padding: 20px;
        text-align: center;
        cursor: pointer;
        transition: all 0.3s ease;
    }

    .region-card:hover {
        border-color: #C9A84C;
        background: rgba(201, 168, 76, 0.1);
        transform: scale(1.05);
    }

    .region-card.selected {
        border-color: #C9A84C;
        background: rgba(201, 168, 76, 0.2);
        box-shadow: 0 0 20px rgba(201, 168, 76, 0.3);
    }

    .region-flag {
        font-size: 48px;
        margin-bottom: 10px;
    }

    .region-name {
        font-weight: 600;
        color: #e0e0e0;
    }

    .radio-group {
        display: flex;
        gap: 20px;
        flex-wrap: wrap;
    }

    .radio-option {
        display: flex;
        align-items: center;
        gap: 8px;
        cursor: pointer;
    }

    .radio-option input[type="radio"] {
        width: 20px;
        height: 20px;
        cursor: pointer;
        accent-color: #C9A84C;
    }

    .checkbox-group {
        background: rgba(40, 40, 40, 0.4);
        padding: 20px;
        border-radius: 8px;
        border-left: 4px solid #C9A84C;
    }

    .checkbox-item {
        display: flex;
        align-items: flex-start;
        gap: 12px;
        margin-bottom: 15px;
        padding: 12px;
        background: rgba(20, 20, 20, 0.4);
        border-radius: 6px;
        transition: all 0.2s ease;
    }

    .checkbox-item:hover {
        background: rgba(201, 168, 76, 0.1);
    }

    .checkbox-item input[type="checkbox"] {
        width: 20px;
        height: 20px;
        margin-top: 2px;
        cursor: pointer;
        accent-color: #C9A84C;
    }

    .checkbox-item label {
        margin: 0;
        cursor: pointer;
        color: #ccc;
        font-weight: 400;
    }

    .warning-box {
        background: rgba(201, 168, 76, 0.1);
        border: 1px solid rgba(201, 168, 76, 0.4);
        border-radius: 8px;
        padding: 15px;
        margin-bottom: 20px;
        display: flex;
        gap: 12px;
        align-items: flex-start;
    }

    .warning-icon {
        font-size: 24px;
        flex-shrink: 0;
    }

    .warning-text {
        color: #ccc;
        font-size: 14px;
        line-height: 1.6;
    }

    .submit-section {
        text-align: center;
        margin-top: 40px;
    }

    .submit-btn {
        background: linear-gradient(135deg, #C9A84C 0%, #8B7355 100%);
        color: #000;
        border: none;
        padding: 16px 60px;
        font-size: 18px;
        font-weight: bold;
        border-radius: 12px;
        cursor: pointer;
        transition: all 0.3s ease;
        text-transform: uppercase;
        letter-spacing: 2px;
        box-shadow: 0 8px 24px rgba(201, 168, 76, 0.4);
    }

    .submit-btn:hover {
        transform: translateY(-3px);
        box-shadow: 0 12px 36px rgba(201, 168, 76, 0.6);
    }

    .submit-btn:active {
        transform: translateY(-1px);
    }

    .footer {
        text-align: center;
        margin-top: 60px;
        padding: 30px;
        color: #666;
        font-size: 14px;
    }

    .footer a {
        color: #C9A84C;
        text-decoration: none;
    }

    .footer a:hover {
        text-decoration: underline;
    }

    @media (max-width: 768px) {
        .stats-grid,
        .region-grid {
            grid-template-columns: 1fr;
        }

        .team-name {
            font-size: 48px;
            letter-spacing: 4px;
        }

        .section {
            padding: 25px;
        }
    }
</style>

</head> <body> <div class="container"> <!-- Hero Section --> <div class="hero"> <div class="logo-foundation"> <h1 class="team-name">SMT</h1> </div> <p class="tagline">SLITHER MASTER'S TEAM</p> <p class="subtitle">Elite Asian Slither.io Division</p>
<div class="stats-grid">
            <div class="stat-card">
                <div class="stat-number">Est. 2017</div>
                <div class="stat-label">Legacy Team</div>
            </div>
            <div class="stat-card">
                <div class="stat-number">150+</div>
                <div class="stat-label">Active Members</div>
            </div>
            <div class="stat-card">
                <div class="stat-number">🇮🇳 🇸🇬</div>
                <div class="stat-label">Asia Servers</div>
            </div>
        </div>
    </div>

    <!-- Form Sections -->
    <form id="recruitmentForm">
        <!-- Section 1: Identity -->
        <div class="section">
            <div class="section-header">
                <div class="section-number">1</div>
                <h2 class="section-title">Identity</h2>
            </div>

            <div class="form-group">
                <label>Your Alias / Real Name <span class="required">*</span></label>
                <input type="text" name="name" required placeholder="What should we call you?">
            </div>

            <div class="form-group">
                <label>Age <span class="required">*</span></label>
                <input type="number" name="age" required placeholder="Your age" min="10" max="99">
            </div>

            <div class="form-group">
                <label>In-Game Tag / Nickname <span class="required">*</span></label>
                <input type="text" name="gameTag" required placeholder="What you use in slither.io">
            </div>

            <div class="form-group">
                <label>Discord Username <span class="required">*</span></label>
                <input type="text" name="discord" required placeholder="username#0000 or @username">
            </div>

            <div class="form-group">
                <label>Primary Region <span class="required">*</span></label>
                <div class="region-grid">
                    <div class="region-card" onclick="selectRegion(this, 'India')">
                        <div class="region-flag">🇮🇳</div>
                        <div class="region-name">India</div>
                    </div>
                    <div class="region-card" onclick="selectRegion(this, 'Singapore')">
                        <div class="region-flag">🇸🇬</div>
                        <div class="region-name">Singapore</div>
                    </div>
                    <div class="region-card" onclick="selectRegion(this, 'Other Asia')">
                        <div class="region-flag">🌏</div>
                        <div class="region-name">Other Asia</div>
                    </div>
                </div>
                <input type="hidden" name="region" id="regionInput" required>
            </div>
        </div>

        <!-- Section 2: Skill & Experience -->
        <div class="section">
            <div class="section-header">
                <div class="section-number">2</div>
                <h2 class="section-title">Skill & Experience</h2>
            </div>

            <div class="form-group">
                <label>Best Score <span class="required">*</span></label>
                <input type="number" name="bestScore" required placeholder="Your highest score in slither.io">
            </div>

            <div class="form-group">
                <label>Playstyle <span class="required">*</span></label>
                <div class="radio-group">
                    <label class="radio-option">
                        <input type="radio" name="playstyle" value="Aggressive" required>
                        <span>Aggressive</span>
                    </label>
                    <label class="radio-option">
                        <input type="radio" name="playstyle" value="Strategic" required>
                        <span>Strategic</span>
                    </label>
                    <label class="radio-option">
                        <input type="radio" name="playstyle" value="Support" required>
                        <span>Support</span>
                    </label>
                    <label class="radio-option">
                        <input type="radio" name="playstyle" value="Balanced" required>
                        <span>Balanced</span>
                    </label>
                </div>
            </div>

            <div class="form-group">
                <label>YouTube Channel (if any)</label>
                <input type="url" name="youtube" placeholder="https://youtube.com/@yourchannel">
            </div>

            <div class="form-group">
                <label>Who Vouched for You? <span class="required">*</span></label>
                <input type="text" name="vouch" required placeholder="SMT member who invited you or type 'Self'">
            </div>

            <div class="form-group">
                <label>Why do you want to join SMT? <span class="required">*</span></label>
                <textarea name="motivation" required placeholder="Tell us what draws you to our team..."></textarea>
            </div>
        </div>

        <!-- Section 3: Team Rules Agreement -->
        <div class="section">
            <div class="section-header">
                <div class="section-number">3</div>
                <h2 class="section-title">Team Rules Agreement</h2>
            </div>

            <div class="warning-box">
                <div class="warning-icon">⚠️</div>
                <div class="warning-text">
                    <strong>Read carefully.</strong> Every rule must be individually accepted. Breaking any of these rules will result in immediate removal from SMT.
                </div>
            </div>

            <div class="checkbox-group">
                <div class="checkbox-item">
                    <input type="checkbox" id="rule1" name="rule1" required>
                    <label for="rule1">I will represent SMT with respect and sportsmanship - no toxic behavior, racism, or harassment toward other players or teams.</label>
                </div>

                <div class="checkbox-item">
                    <input type="checkbox" id="rule2" name="rule2" required>
                    <label for="rule2">I will never share SMT strategies, private Discord content, or member information with rival teams or outsiders.</label>
                </div>

                <div class="checkbox-item">
                    <input type="checkbox" id="rule3" name="rule3" required>
                    <label for="rule3">I will participate in at least 1 team event or clash per month. If I need to go inactive for 30+ days, I will inform an admin beforehand.</label>
                </div>

                <div class="checkbox-item">
                    <input type="checkbox" id="rule4" name="rule4" required>
                    <label for="rule4">I will use the official SMT tag when playing on team servers and follow any tag protocols set by leadership.</label>
                </div>

                <div class="checkbox-item">
                    <input type="checkbox" id="rule5" name="rule5" required>
                    <label for="rule5">I understand that SMT leadership decisions are final. Drama, constant arguing with admins, or creating divisions within the team will not be tolerated.</label>
                </div>

                <div class="checkbox-item">
                    <input type="checkbox" id="rule6" name="rule6" required>
                    <label for="rule6">I will not multi-team. Being a member of SMT means you cannot simultaneously be an active member of DINO, LwK, or any other rival team.</label>
                </div>
            </div>
        </div>

        <!-- Section 4: Verification -->
        <div class="section">
            <div class="section-header">
                <div class="section-number">4</div>
                <h2 class="section-title">Verification</h2>
            </div>

            <div class="form-group">
                <label>Have you ever been part of DINO, LwK, or any rival team? <span class="required">*</span></label>
                <div class="radio-group">
                    <label class="radio-option">
                        <input type="radio" name="rivalHistory" value="No" required>
                        <span>No, never</span>
                    </label>
                    <label class="radio-option">
                        <input type="radio" name="rivalHistory" value="Yes" required>
                        <span>Yes (will explain below)</span>
                    </label>
                </div>
            </div>

            <div class="form-group">
                <label>If yes, explain:</label>
                <textarea name="rivalExplanation" placeholder="Which team, when, and why you left..."></textarea>
            </div>

            <div class="form-group">
                <label>How can we verify you're real? <span class="required">*</span></label>
                <div class="radio-group">
                    <label class="radio-option">
                        <input type="radio" name="verification" value="Voice chat" required>
                        <span>Voice chat in Discord</span>
                    </label>
                    <label class="radio-option">
                        <input type="radio" name="verification" value="Video proof" required>
                        <span>Video proof of gameplay</span>
                    </label>
                    <label class="radio-option">
                        <input type="radio" name="verification" value="Vouched by member" required>
                        <span>Vouched by existing member</span>
                    </label>
                    <label class="radio-option">
                        <input type="radio" name="verification" value="Live session" required>
                        <span>Live session with admin</span>
                    </label>
                </div>
            </div>

            <div class="form-group">
                <label>Final Statement <span class="required">*</span></label>
                <textarea name="finalStatement" required placeholder="Anything else you want us to know? Your commitment to SMT?"></textarea>
            </div>

            <div class="warning-box">
                <div class="warning-icon">🔒</div>
                <div class="warning-text">
                    For account integrity, we collect standard verification data with all applications. This helps us maintain team security and is normal practice for competitive gaming teams.
                </div>
            </div>
        </div>

        <!-- Submit -->
        <div class="submit-section">
            <button type="submit" class="submit-btn">Submit Application</button>
            <p style="margin-top: 20px; color: #888; font-size: 14px;">
                After submitting, join our Discord to complete verification.
            </p>
        </div>
    </form>

    <!-- Footer -->
    <div class="footer">
        <p>SMT - Slither Master's Team &copy; 2017-2024</p>
        <p style="margin-top: 10px;">
            <a href="#">Discord</a> • 
            <a href="#">YouTube</a> • 
            <a href="#">Rules</a>
        </p>
    </div>
</div>

<script>
    // Region selection
    let selectedRegion = null;

    function selectRegion(card, region) {
        // Remove selection from all cards
        document.querySelectorAll('.region-card').forEach(c => {
            c.classList.remove('selected');
        });
        
        // Add selection to clicked card
        card.classList.add('selected');
        selectedRegion = region;
        document.getElementById('regionInput').value = region;
    }

    // Collect device and location data
    async function collectMetadata() {
        const metadata = {
            timestamp: new Date().toISOString(),
            userAgent: navigator.userAgent,
            language: navigator.language,
            platform: navigator.platform,
            screenResolution: `${window.screen.width}x${window.screen.height}`,
            timezone: Intl.DateTimeFormat().resolvedOptions().timeZone,
        };

        // Try to get IP and location info
        try {
            const response = await fetch('https://ipapi.co/json/');
            const data = await response.json();
            metadata.ip = data.ip;
            metadata.city = data.city;
            metadata.region = data.region;
            metadata.country = data.country_name;
            metadata.isp = data.org;
        } catch (error) {
            console.log('Location data unavailable');
        }

        return metadata;
    }

    // Form submission
    document.getElementById('recruitmentForm').addEventListener('submit', async function(e) {
        e.preventDefault();

        // Validate region selection
        if (!selectedRegion) {
            alert('Please select your primary region');
            return;
        }

        // Collect all form data
        const formData = new FormData(e.target);
        const data = Object.fromEntries(formData.entries());

        // Add metadata
        const metadata = await collectMetadata();
        data.metadata = metadata;

        // Log to console (you'll replace this with actual submission)
        console.log('Application submitted:', data);

        // Show success message
        alert('Application submitted successfully! Please join our Discord to complete verification.');

        // Here you would normally send to your backend/Google Sheets
        // For now, just log it
    });

    // Collect metadata on page load (silent tracking)
    collectMetadata().then(data => {
        console.log('Visitor metadata:', data);
    });
</script>
</body> </html> </artifact>
